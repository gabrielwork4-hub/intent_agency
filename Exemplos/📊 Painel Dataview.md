---
tipo: dashboard
atualizado: 2026-06-15
---

# 📊 Painel Dataview

> ⚠️ As consultas abaixo só funcionam DEPOIS de instalar e ativar o plugin **Dataview**
> (Settings → Community plugins → Browse → "Dataview" → Install → Enable).
> Sem o plugin, você verá apenas o código. Com ele ativo, vira tabela/lista automática. ✨
>
> O que o Dataview faz: ele LÊ o frontmatter (aqueles campos entre `---`) de todas as
> notas e monta listas/tabelas sozinho. Se você criar um cliente novo amanhã, ele
> aparece aqui automaticamente — sem editar esta nota.

---

## 1️⃣ Lista simples: todos os clientes
Pega toda nota onde `tipo` = `cliente`.

```dataview
LIST
FROM "Exemplos"
WHERE tipo = "cliente"
```

---

## 2️⃣ Tabela: clientes ativos com detalhes
Mostra colunas vindas direto do frontmatter.

```dataview
TABLE status, segmento, responsavel, inicio_contrato AS "Início"
FROM "Exemplos"
WHERE tipo = "cliente" AND status = "ativo"
```

---

## 3️⃣ Projetos por prioridade
Lista projetos ordenados, mostrando cliente e prazo.

```dataview
TABLE cliente, status, prioridade, prazo
FROM "Exemplos"
WHERE tipo = "projeto"
SORT prioridade ASC
```

---

## 4️⃣ Tarefas pendentes de todos os projetos
O Dataview varre os checkboxes `- [ ]` de TODAS as notas e junta aqui as não-concluídas.

```dataview
TASK
FROM "Exemplos"
WHERE !completed
```

---

## 5️⃣ Toda a base de conhecimento
```dataview
LIST
FROM "Exemplos"
WHERE tipo = "conhecimento"
```

---

## Como ler a sintaxe (resumo)
- `LIST` / `TABLE` / `TASK` → o formato da saída
- `FROM "pasta"` ou `FROM #tag` → de onde puxar
- `WHERE` → o filtro (igual a um `WHERE` de SQL)
- `SORT` → ordenação

🏠 Voltar: [[🏠 Painel Central]]

#dataview #seo
