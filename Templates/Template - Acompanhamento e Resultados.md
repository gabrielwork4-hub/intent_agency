<%*
const nome = await tp.system.prompt("Nome do cliente (para o acompanhamento)");
await tp.file.rename("Acompanhamento - " + nome);
-%>
---
tipo: acompanhamento
cliente: "[[<% nome %>]]"
status: ativo
atualizado: <% tp.date.now("YYYY-MM-DD") %>
tags: [acompanhamento, resultados]
---

# 📊 Acompanhamento e Resultados — <% nome %>

> Fecha o ciclo de validação: **baseline → metas → ações → resultados → aprendizados**.
> Atualizar na cadência de revisão. Fonte para provar o que funcionou e calibrar a estratégia.

## 📏 Baseline (ponto de partida)
> Snapshot do início — sem isso não há como medir evolução. Registrar data.
- Data do baseline: <% tp.date.now("YYYY-MM-DD") %>
- Posições/keywords-chave: 
- Tráfego orgânico (GSC): 
- Conversões/leads por mês: 
- Avaliações (nota / volume): 
- Observações técnicas: 

## 🎯 Metas
> O que define sucesso. Concretas e mensuráveis.
- Meta principal: 
- KPIs: 
- Prazo: 

## 🕒 Registro de ações (timeline)
> O que foi feito e QUANDO — base para atribuição (o que causou o quê).
| Data | Ação | Metodologia | Resultado esperado |
|---|---|---|---|
|  |  |  |  |

## 📈 Resultados ao longo do tempo
> Medição periódica (mensal). Conecta com report no Looker Studio.
| Mês | Posições | Tráfego | Leads/conversões | Avaliações | Nota |
|---|---|---|---|---|---|
|  |  |  |  |  |  |

## 🧪 Hipóteses / experimentos
> "Acreditamos que X → faremos Y → esperamos Z." Validar e mover aprendizado para [[Aprendizados Validados]].
- [ ] Hipótese: … → Ação: … → Esperado: … → **Resultado:** (pendente)

## 🧠 Aprendizados deste cliente
> O que validamos aqui. Promover os reutilizáveis para [[Aprendizados Validados]].
- 

---
🔗 Relacionado: [[<% nome %>]] · [[Aprendizados Validados]]
