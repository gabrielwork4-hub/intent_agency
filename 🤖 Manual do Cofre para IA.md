---
tipo: manual-ia
papel: orientação para o Claude consultar e atuar a partir do cofre
atualizado: 2026-06-15
tags: [ia, manual, rag]
---

# 🤖 Manual do Cofre para IA

> Leia esta nota ao começar a trabalhar com este cofre. Ela explica o que é a base,
> como está organizada e como você (Claude) deve usá-la para atuar nas demandas dos clientes.

## 🎯 O que é este cofre
Centralizador de informações e **base de inteligência dos clientes** que o Gabriel atende.
Serve como material de consulta (RAG) para a IA atuar nas demandas: SEO, geração de
demanda qualificada, estratégia, conteúdo.

## 🧭 Por onde começar
1. **[[🗺️ Índice Mestre]]** — mapa de tudo. Sempre comece por aqui.
2. **[[00 - Guia e Convenções do Cofre]]** — padrões de estrutura e frontmatter.
3. A pasta **/Clientes** — uma subnota por cliente, com ICP/Escopo/Projetos linkados.

## 🗂️ Como o cofre é organizado
- `/Clientes` — inteligência por cliente. Cada cliente tem nota principal + notas
  satélite (`ICP - `, `Escopo - `, `Projeto - `) conectadas por `[[links]]`.
- `/Conhecimento` — metodologias e referências reutilizáveis entre clientes.
- Raiz — índice mestre, guia, este manual.
- `/Exemplos` — material de aprendizado, ignorar para fins de trabalho real.

## 🔎 Como recuperar informação (fluxo recomendado)
1. Abra [[🗺️ Índice Mestre]] para localizar o cliente/assunto.
2. Abra a nota principal do cliente; siga os `[[links]]` (ICP, Escopo, Projeto).
3. Use o **frontmatter** para filtrar (`tipo`, `status`, `vinculo`, `segmento`).
4. Cite/baseie-se sempre no conteúdo do cofre — não invente dados de cliente.

## 📋 Convenções que você deve seguir ao escrever no cofre
- Respeite o padrão de frontmatter do [[00 - Guia e Convenções do Cofre]].
- Notas **atômicas** (1 assunto), título descritivo, resumo em `>` no topo.
- Conteúdo **auto-contido** (sem "isso/ele" ambíguo) — pensado para ser lido em pedaços.
- Linke com `[[ ]]` e atualize o [[🗺️ Índice Mestre]] quando criar algo relevante.
- Campos sem informação: deixe em branco/placeholder — **nunca preencha com suposição.**

## 🚦 Status atual dos clientes
- **Mari Quitutes** (confeitaria, agência) — ativo · ICP + Projeto SEO mapeados
- **Gold Car** (mecânica, agência) — ativo · ICP + Projeto SEO mapeados (inclui contexto técnico)
- **ID Singular** (consultoria/educação corporativa, PJ) — em início · ICP + Escopo mapeados

## ⚠️ Sensibilidade de dados
Dados sigilosos (contratos, financeiro, documentos pessoais) **não devem entrar no cofre**.
O cofre contém estratégia, ICP, escopo e conhecimento — não dados confidenciais.

🔗 Relacionado: [[🗺️ Índice Mestre]] · [[00 - Guia e Convenções do Cofre]]

#ia #manual #rag
