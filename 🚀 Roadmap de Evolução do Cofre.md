---
tipo: roadmap
papel: plano de evolução do cofre alinhado à operação
atualizado: 2026-06-16
tags: [roadmap, melhorias, sistema]
---

# 🚀 Roadmap de Evolução do Cofre

> Plano de melhorias e inovações do cofre, **alinhado à operação** (clientes + metodologias +
> ciclo de validação). Documento vivo: priorizar por fase, marcar status, e evoluir.
> Status: ⬜ a fazer · 🔄 em andamento · ✅ feito.

## 🎯 Objetivo
Tornar o cofre um sistema "parrudo": rápido de operar, consistente (RAG melhor), com dashboards
que dão visão e automações que poupam tempo — sem perder a simplicidade do markdown + Git.

## 🧭 Princípios
- Cada melhoria deve **servir a operação** (clientes/metodologias/validação), não ser enfeite.
- Markdown puro + Git como base (sem lock-in).
- Construir em fases — sentir valor antes de somar a próxima.

---

## 📐 FASE 1 — Fundação de produtividade
> Maior alavancagem: multiplica tudo que já construímos.

### 1.1 Dataview ✅
- **O que:** plugin que consulta o frontmatter como banco de dados.
- **Valor p/ operação:** ativa os painéis automáticos (clientes ativos, tarefas, resultados).
- **Status:** instalado e ativo (v0.5.68). Painéis renderizando.

### 1.2 Templater + pasta /Templates 🔄
- **O que:** criação de notas já padronizadas (cliente, projeto, acompanhamento, brief).
- **Valor p/ operação:** todo cliente novo nasce com ICP + Projeto + Acompanhamento num clique.
  Consistência = assertividade + RAG melhor.
- **Esforço:** médio. **Depende de:** instalar Templater + configurar pasta.
- ✅ **Templates criados:** Cliente, ICP, Projeto, Acompanhamento, Brief de Conteúdo (ver [[📋 Templates]]).
- ⬜ **Falta:** instalar plugin Templater e apontar a pasta `Templates` nas configurações.

### 1.3 Cores no Graph View + Hotkeys ⬜
- **O que:** pintar nós por pasta/tipo; atalhos para comandos frequentes.
- **Valor p/ operação:** navegação rápida e leitura visual da estrutura.
- **Esforço:** baixo.

---

## 📊 FASE 2 — Dashboards (visão da operação)
> Requer Dataview (Fase 1).

### 2.1 Central de Comando ✅
- **O que:** nota-painel que mostra automaticamente: clientes, projetos, tarefas pendentes,
  acompanhamentos e status das metodologias.
- **Valor p/ operação:** visão única do dia — o que fazer agora, em qual cliente.
- **Status:** criada em [[🧭 Central de Comando]] (ativa com Dataview).

### 2.2 Pipeline de Conteúdo ⬜
- **O que:** status de cada página/pauta (a fazer → escrevendo → publicado → ranqueando).
- **Valor p/ operação:** controle da produção de conteúdo (Metodologias #2/#3/#4).
- **Esforço:** médio. **Depende de:** padronizar frontmatter de notas de conteúdo.

### 2.3 Visão de Resultados ⬜
- **O que:** tabela única com baseline + métricas de todos os clientes.
- **Valor p/ operação:** fecha o ciclo de validação; prova de resultado num lugar só.
- **Esforço:** médio. **Depende de:** acompanhamentos preenchidos.

---

## 🎨 FASE 3 — Visualização e fluxo
### 3.1 Kanban (pipeline) ⬜
- **O que:** quadro visual de tarefas/conteúdo por cliente.
- **Valor p/ operação:** gestão visual quando a produção crescer.
- **Esforço:** baixo-médio.

### 3.2 Canvas / Excalidraw (mapas de estratégia) ⬜
- **O que:** mapa visual ICP → clusters → páginas (com setas); funis/jornadas.
- **Valor p/ operação:** desenhar estratégia por cliente de forma visual.
- **Esforço:** médio.

---

## 🤖 FASE 4 — Automação e captura
### 4.1 QuickAdd ⬜
- **O que:** capturar ideia/keyword rápido sem abrir nota.
- **Valor p/ operação:** não perder insights no meio da execução.
### 4.2 Ajuste fino do Obsidian Git ⬜
- **O que:** revisar intervalo de commit para histórico mais limpo.
- **Valor p/ operação:** versionamento organizado.

---

## 💡 FASE 5 — Inovações (RAG + agência)
### 5.1 Clusters de keywords como dados no cofre ⬜
- **O que:** registrar a planilha clusterizada dentro do Obsidian (Dataview consulta).
- **Valor p/ operação:** o estudo de palavras entra no RAG; eu (Claude) consulto direto.
### 5.2 Biblioteca de copy validado ("snippets") ⬜
- **O que:** trechos de copy que converteram, reutilizáveis.
- **Valor p/ operação:** acelera produção e melhora qualidade (liga em [[Aprendizados Validados]]).
### 5.3 Revisões agendadas (cadência) ⬜
- **O que:** ritmo mensal por cliente + template de report.
- **Valor p/ operação:** alimenta o ciclo de validação de forma consistente.

---

## 🗺️ Ordem recomendada
1. **Fase 1** (Dataview + Templater) — base que multiplica tudo
2. **Fase 2.1** (Central de Comando) — visão imediata da operação
3. **Fase 2.3** (Visão de Resultados) — fecha a validação
4. Demais conforme a operação pedir

## 📊 Resumo (visão rápida)
| Fase | Item | Esforço | Status |
|---|---|---|---|
| 1 | Dataview | baixo | ✅ |
| 1 | Templater + Templates | médio | 🔄 (falta apontar pasta) |
| 1 | Graph cores + Hotkeys | baixo | 🔄 (Hotkeys++ instalado) |
| 2 | Central de Comando | médio | ✅ |
| 2 | Pipeline de Conteúdo | médio | ⬜ |
| 2 | Visão de Resultados | médio | ⬜ |
| 3 | Kanban | baixo-médio | ⬜ |
| 3 | Canvas/Excalidraw | médio | ⬜ |
| 4 | QuickAdd | baixo | ⬜ |
| 4 | Ajuste Git | baixo | ⬜ |
| 5 | Clusters como dados | médio | ⬜ |
| 5 | Biblioteca de copy | baixo | ⬜ |
| 5 | Revisões agendadas | médio | ⬜ |

---
🔗 Relacionado: [[🗺️ Índice Mestre]] · [[📚 Conhecimento]] · [[🤖 Manual do Cofre para IA]]

#roadmap #melhorias #sistema
