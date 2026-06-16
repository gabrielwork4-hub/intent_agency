---
tipo: dashboard
papel: visão consolidada de resultados e validação (Dataview)
atualizado: 2026-06-16
tags: [dashboard, resultados, validacao]
---

# 📈 Visão de Resultados

> Consolida o ciclo de validação de todos os clientes. Atualiza sozinho.
> Cada cliente tem um acompanhamento detalhado (baseline → metas → ações → resultados).

## 📊 Acompanhamentos por cliente
```dataview
TABLE cliente, status, atualizado
FROM "Clientes"
WHERE tipo = "acompanhamento"
SORT atualizado DESC
```

## 📁 Projetos em andamento (o que está sendo executado)
```dataview
TABLE cliente, foco, prioridade, status
FROM "Clientes"
WHERE tipo = "projeto"
SORT status ASC, prioridade ASC
```

## 🧪 Hipóteses em aberto (a validar)
```dataview
TASK
FROM "Clientes"
WHERE tipo = "acompanhamento" AND !completed
GROUP BY file.link
```

## 🧠 Aprendizados acumulados
- [[Aprendizados Validados]] — o que já validamos e realimentou as metodologias

---
> 💡 As métricas detalhadas (posições, tráfego, leads) ficam dentro de cada acompanhamento.
> À medida que preenchermos os resultados mensais, esta visão vira o "placar" da operação.

🔗 Relacionado: [[🧭 Central de Comando]] · [[Acompanhamento - Gold Car]] · [[Acompanhamento - Mari Quitutes]] · [[Acompanhamento - ID Singular]]

#dashboard #resultados #validacao
