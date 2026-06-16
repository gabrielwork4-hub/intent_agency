---
tipo: guia
atualizado: 2026-06-15
tags: [guia, convencoes, rag]
---

# 00 - Guia e Convenções do Cofre

> Esta é a **base de padronização** do cofre. Objetivo: organização clara para uso humano
> **e** como fonte de RAG (recuperação por IA). Toda nota nova deve seguir estas convenções.

## 🎯 Por que padronizar (foco RAG)
O RAG quebra notas em **pedaços (chunks)** e recupera os mais relevantes. Notas bem
estruturadas = respostas melhores. Regras de ouro:

1. **Atômica** — 1 conceito por nota. Se a nota fala de 2 assuntos, divida.
2. **Título descritivo e único** — diz o que é só pelo nome.
3. **Resumo no topo** — primeiras linhas explicam a nota (usar `>` citação).
4. **Headings `##` claros** — funcionam como fronteira de chunk.
5. **Auto-contido** — evitar "ele/isso/como falamos"; o trecho pode ser lido sozinho.
6. **Vocabulário consistente** — mesmo termo para a mesma coisa, sempre.

---

## 📁 Estrutura de pastas
```
/                         → guia, índices (MOC)
/Clientes                 → uma nota por cliente + ICP/Escopo/Projetos
/Conhecimento             → notas reutilizáveis (metodologias, checklists, referências)
/Projetos                 → projetos que não são de um cliente único (opcional)
/Templates                → modelos de nota (Templater)
/Exemplos                 → notas de aprendizado (apagar quando quiser)
```

> Lembrete da filosofia: **pastas organizam, links conectam.** Não sofra com "onde guardar";
> conecte com `[[ ]]`.

---

## 🏷️ Padrão de frontmatter
Todo arquivo começa com metadados entre `---`. Campos por tipo:

**Cliente**
```yaml
tipo: cliente
nome:
segmento:
status: ativo | em início | pausado | encerrado
vinculo: agência (Intent Marketing) | PJ
responsavel:
inicio_contrato:
tags: [cliente]
```

**Projeto**
```yaml
tipo: projeto
cliente: "[[Nome do Cliente]]"
status: em início | em andamento | concluído
prioridade: alta | média | baixa
prazo:
tags: [projeto]
```

**Conhecimento**
```yaml
tipo: conhecimento
categoria:
tags: [conhecimento]
```

### Valores padronizados (sempre usar estes)
- **status:** `ativo`, `em início`, `em andamento`, `pausado`, `concluído`, `encerrado`
- **prioridade:** `alta`, `média`, `baixa`
- **vinculo:** `agência (Intent Marketing)`, `PJ`
- **tipo:** `cliente`, `projeto`, `conhecimento`, `icp`, `escopo`, `guia`, `dashboard`

---

## 📝 Anatomia de uma nota (modelo mental)
```markdown
---
(frontmatter)
---

# Título Descritivo

> Resumo em 1-2 linhas: o que é esta nota e para que serve.

## Seção 1
Conteúdo auto-contido...

## Seção 2
...

🔗 Relacionado: [[Outra Nota]] · [[Mais Uma]]

#tags #relevantes
```

---

## 🔤 Convenções de nome de arquivo
- Use nomes claros: `ICP - ID Singular`, `Projeto - SEO Gold Car`.
- Prefixos por tipo ajudam a achar: `Cliente - `, `Projeto - `, `Conhecimento - `.
- Evite nomes genéricos ("Notas", "Sem título").

---

## 🔗 Links e tags
- Linke generosamente com `[[ ]]` — inclusive notas que ainda não existem.
- Tags em minúsculo, sem acento quando possível: `#geracao-de-demanda`.
- Use tags aninhadas para hierarquia: `#cliente/ativo`.

🔗 Relacionado: [[🏠 Painel Central]]

#guia #convencoes #rag
