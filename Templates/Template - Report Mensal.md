<%*
const cliente = await tp.system.prompt("Nome do cliente");
const mes = await tp.system.prompt("Mês de referência (ex: 2026-06)");
await tp.file.rename("Report " + mes + " - " + cliente);
-%>
---
tipo: report-mensal
cliente: "[[<% cliente %>]]"
mes: <% mes %>
atualizado: <% tp.date.now("YYYY-MM-DD") %>
tags: [report, resultados]
---

# 📊 Report <% mes %> — <% cliente %>

> Resumo mensal de resultados. Segue [[Cadência de Revisão]].

## 🎯 Destaques do mês
- 

## 📈 Números
| Métrica | Mês anterior | Este mês | Meta | Δ |
|---|---|---|---|---|
| Posições-chave |  |  |  |  |
| Tráfego orgânico |  |  |  |  |
| Leads/conversões |  |  |  |  |
| Avaliações (nota/vol.) |  |  |  |  |

## ✅ O que foi feito
- 

## 🧪 Hipóteses validadas
- 

## ➡️ Próximas ações
- [ ] 

---
🔗 Relacionado: [[<% cliente %>]] · [[Acompanhamento - <% cliente %>]]

#report #resultados
