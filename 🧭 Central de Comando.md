---
tipo: dashboard
papel: visão única da operação (Dataview)
atualizado: 2026-06-16
tags: [dashboard, central, operacao]
---

# 🧭 Central de Comando

> Visão única da operação — atualiza sozinha (Dataview). O que está ativo, o que fazer,
> e o estado de cada frente. Ponto de partida do dia.

## 👥 Clientes ativos
```dataview
TABLE segmento, vinculo, foco, status
FROM "Clientes"
WHERE tipo = "cliente"
SORT status ASC
```

## 📁 Projetos
```dataview
TABLE cliente, foco, prioridade, status
FROM "Clientes"
WHERE tipo = "projeto"
SORT prioridade ASC, status ASC
```

## ✅ Tarefas pendentes (todos os clientes)
```dataview
TASK
FROM "Clientes"
WHERE !completed
GROUP BY file.link
```

## 📊 Acompanhamentos (ciclo de validação)
```dataview
TABLE cliente, status, atualizado
FROM "Clientes"
WHERE tipo = "acompanhamento"
SORT atualizado DESC
```

## 🧠 Metodologias (status)
```dataview
TABLE etapa AS "#", fase, status
FROM "Conhecimento"
WHERE tipo = "metodologia"
SORT etapa ASC
```

## 🚀 Evolução do cofre
- [[🚀 Roadmap de Evolução do Cofre]] — fases de melhoria

---
🔗 Relacionado: [[🗺️ Índice Mestre]] · [[👥 Clientes]] · [[📚 Conhecimento]]

#dashboard #central
