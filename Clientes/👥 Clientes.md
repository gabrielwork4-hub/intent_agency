---
tipo: dashboard
atualizado: 2026-06-15
---

# 👥 Clientes

Índice dos clientes ativos. Sou responsável pelas estratégias de todos abaixo.

## Agência (Intent Marketing)
- [[Mari Quitutes]] — confeitaria
- [[Gold Car]] — mecânica

## PJ (fora da Intent Marketing)
- [[ID Singular]] — geração de demanda qualificada · *em início*

---

## 📊 Painel automático (requer Dataview)
Esta tabela se atualiza sozinha conforme você cria/edita notas de cliente.

```dataview
TABLE segmento, status, funcao AS "Minha função", cidade
FROM "Clientes"
WHERE tipo = "cliente"
SORT nome ASC
```

#clientes #seo
