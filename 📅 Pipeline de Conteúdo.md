---
tipo: dashboard
papel: pipeline de produção de conteúdo (Dataview)
atualizado: 2026-06-16
tags: [dashboard, conteudo, pipeline]
---

# 📅 Pipeline de Conteúdo

> Controle da produção de conteúdo (briefs/páginas/pautas). Atualiza sozinho conforme os
> briefs mudam de `status`. Liga em [[Metodologia - Brief para Produção de Artigos e Páginas]].
>
> **Status de conteúdo:** `a fazer` → `escrevendo` → `em revisão` → `publicado` → `ranqueando`.

## 🗂️ Visão geral (por cliente e status)
```dataview
TABLE cliente, destino, status, atualizado
FROM "Clientes"
WHERE tipo = "brief-conteudo"
SORT status ASC, cliente ASC
```

## ✍️ A fazer
```dataview
LIST
FROM "Clientes"
WHERE tipo = "brief-conteudo" AND status = "a fazer"
```

## 🛠️ Em produção (escrevendo / em revisão)
```dataview
TABLE cliente, status
FROM "Clientes"
WHERE tipo = "brief-conteudo" AND (status = "escrevendo" OR status = "em revisão")
```

## ✅ Publicado / Ranqueando
```dataview
TABLE cliente, status, atualizado
FROM "Clientes"
WHERE tipo = "brief-conteudo" AND (status = "publicado" OR status = "ranqueando")
SORT atualizado DESC
```

---
> 💡 Os briefs ainda não existem — este painel popula sozinho conforme você criar peças
> pelo [[📋 Templates|Template - Brief de Conteúdo]].

🔗 Relacionado: [[🧭 Central de Comando]] · [[🗺️ Índice Mestre]]

#dashboard #conteudo #pipeline
