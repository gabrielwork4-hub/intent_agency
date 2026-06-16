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

### 1.2 Templater + pasta /Templates ✅
- **O que:** criação de notas já padronizadas (cliente, projeto, acompanhamento, brief).
- **Valor p/ operação:** todo cliente novo nasce com ICP + Projeto + Acompanhamento num clique.
- **Status:** Templater ativo + pasta configurada. 5 templates **inteligentes** (perguntam nome,
  renomeiam e preenchem links sozinhos) — ver [[📋 Templates]]. Testado e funcionando.

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

### 2.2 Pipeline de Conteúdo ✅
- **O que:** status de cada página/pauta (a fazer → escrevendo → em revisão → publicado → ranqueando).
- **Valor p/ operação:** controle da produção de conteúdo (Metodologias #2/#3/#4).
- **Status:** criado em [[📅 Pipeline de Conteúdo]]; status padronizado no template de Brief e no guia.

### 2.3 Visão de Resultados ✅
- **O que:** consolida acompanhamentos, projetos em execução e hipóteses em aberto.
- **Valor p/ operação:** fecha o ciclo de validação; placar da operação num lugar só.
- **Status:** criado em [[📈 Visão de Resultados]].

---

## 🎨 FASE 3 — Visualização e fluxo
### 3.1 Kanban (pipeline) ⬜ *(depende de instalar plugin Kanban)*
- **O que:** quadro visual de tarefas/conteúdo por cliente.
- **Nota:** o [[📅 Pipeline de Conteúdo]] (Dataview) já cobre isso. Kanban é alternativa visual opcional.

### 3.2 Canvas / Excalidraw (mapas de estratégia) ⬜ *(manual)*
- **O que:** mapa visual ICP → clusters → páginas (com setas); funis/jornadas.
- **Nota:** Canvas é nativo; montar manualmente por cliente quando precisar.

---

## 🤖 FASE 4 — Automação e captura
### 4.1 QuickAdd 🔄 *(estrutura pronta; falta instalar plugin)*
- **O que:** capturar ideia/keyword rápido sem abrir nota.
- **Status:** inbox criado em [[📥 Captura]] com instruções. Falta instalar o plugin QuickAdd.
### 4.2 Ajuste fino do Obsidian Git ⬜
- **O que:** revisar intervalo de commit (hoje 1 min) para ~5–10 min → histórico mais limpo.
- **Valor p/ operação:** versionamento organizado. *(ajuste de configuração — você faz)*

---

## 💡 FASE 5 — Inovações (RAG + agência)
### 5.1 Clusters de keywords como dados no cofre ✅
- **O que:** registrar clusters como notas (Dataview consulta) — entra no RAG.
- **Status:** [[📋 Templates|Template - Cluster de Keywords]] criado (serviço + pauta amarrados).
### 5.2 Biblioteca de copy validado ("snippets") ✅
- **O que:** trechos de copy que converteram, reutilizáveis.
- **Status:** criada em [[Biblioteca de Copy]].
### 5.3 Revisões agendadas (cadência) ✅
- **O que:** ritmo mensal por cliente + template de report.
- **Status:** [[Cadência de Revisão]] + [[📋 Templates|Template - Report Mensal]] criados.

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
| 1 | Templater + Templates | médio | ✅ |
| 1 | Graph cores + Hotkeys | baixo | 🔄 (Hotkeys++ instalado) |
| 2 | Central de Comando | médio | ✅ |
| 2 | Pipeline de Conteúdo | médio | ✅ |
| 2 | Visão de Resultados | médio | ✅ |
| 3 | Kanban | baixo-médio | ⬜ (opcional, requer plugin) |
| 3 | Canvas/Excalidraw | médio | ⬜ (manual, quando precisar) |
| 4 | QuickAdd | baixo | 🔄 (estrutura ✅, falta plugin) |
| 4 | Ajuste Git | baixo | ⬜ (você ajusta) |
| 5 | Clusters como dados | médio | ✅ |
| 5 | Biblioteca de copy | baixo | ✅ |
| 5 | Revisões agendadas | médio | ✅ |

---
🔗 Relacionado: [[🗺️ Índice Mestre]] · [[📚 Conhecimento]] · [[🤖 Manual do Cofre para IA]]

#roadmap #melhorias #sistema
