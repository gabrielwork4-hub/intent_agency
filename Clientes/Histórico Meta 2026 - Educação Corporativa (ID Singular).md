---
tipo: historico-performance
cliente: "[[ID Singular]]"
canal: Meta Ads
periodo: jan-jun/2026
fonte: export Conjuntos de Anúncios (Meta Ads Manager)
atualizado: 2026-06-29
tags: [historico, meta-ads, educacao-corporativa, id-singular, performance]
---

# 📊 Histórico Meta Ads — Educação Corporativa (jan-jun/2026)

> Granularidade por conjunto de anúncios (Meta, jan-jun/2026). Complementa o baseline blended
> registrado em [[Acompanhamento - ID Singular]] (52 leads · R$28.877,60 · CPL R$555,34 — esse
> número é **blended dos 3 canais**: Meta+Google+LinkedIn). Aqui é **só Meta**.

## 🔑 Achado principal
**Meta isolado é muito mais eficiente que o blended:** CPL R$233,85 (Meta) vs. R$555,34 (blended
3 canais) — confirma que **Google e/ou LinkedIn estavam puxando a média pra cima** nesse período.
Mesmo padrão observado em Liderança (Meta é o canal mais barato/eficiente do mix da ID Singular).

## 📋 Conjuntos de anúncios (Meta, jan-jun/2026)
| Conjunto | Status | Leads | Custo/Lead | Gasto | Impressões | Alcance | Orçamento/dia |
|---|---|---|---|---|---|---|---|
| **(CJ1) Leads Página de Vendas** | not_delivering | 22 | **R$104,32** ⭐ melhor CPL do lote | R$2.294,93 | 27.896 | 15.958 | R$60,77 |
| publicosegmentadoRH | not_delivering | 27 | R$250,68 | R$6.768,29 | 103.224 | 61.970 | R$90,00 |
| publicoabertoadv_lp_captura | inactive | 8 | R$355,17 | R$2.841,34 | 27.503 | 16.058 | R$60,00 |
| (CJ1) LAL 1% (LP + Captura) | inactive | 0 | — | R$74,56 | 2.716 | 2.279 | R$17,96 |
| publicoabertoadv_lp_captura_02 | inactive | 0 | — | R$614,26 | 5.889 | 3.497 | R$60,00 |
| saudemental | not_delivering | 0 | — | R$735,84 | 6.008 | 3.509 | R$51,00 |
| **TOTAL** | | **57** | **R$233,85 (blended Meta)** | **R$13.329,22** | 173.236 | 103.271 | — |

## 🧠 Leitura por conjunto
- **(CJ1) Leads Página de Vendas — melhor desempenho de todos.** CPL R$104,32, menos de metade do
  blended Meta. Público/criativo desse conjunto é o benchmark a replicar em campanhas novas
  (Educação Financeira, próximos lançamentos).
- **publicosegmentadoRH — maior volume (27 leads), CPL moderado (R$250,68).** Segmentação por cargo
  (RH) funciona, mas é ~2,4× mais cara que o conjunto acima — vale testar reduzir o público pra mais
  qualificado, ou aplicar o criativo do "Leads Página de Vendas" nesse público.
- **publicoabertoadv_lp_captura — CPL alto (R$355,17), poucos leads (8).** Público aberto (sem
  segmentação por advocacia/RH) tende a custar mais — confirma padrão: público aberto > público
  segmentado em custo de aquisição.
- **3 conjuntos com 0 leads** (LAL 1%, captura_02, saudemental) — gastaram R$1.424,66 combinados sem
  nenhum resultado atribuído. Podem ter o mesmo problema de tracking que identificamos em Liderança
  (pixel/evento não configurado), ou simplesmente não geraram demanda — **a investigar se vale revisar
  a tag desses conjuntos também, já que a causa raiz (trigger antigo "btn-educorp-enviar-lv1") era
  justamente do formulário de Educação Corporativa.**

## 🎯 Implicações para o planejamento de julho
1. **Meta deve receber a maior fatia do orçamento** para Educação Corporativa/Financeira — é o canal
   comprovadamente mais eficiente (mesmo padrão de Liderança: Meta R$6.500 de R$9.000 total).
2. **Replicar a estratégia de público/criativo de "(CJ1) Leads Página de Vendas"** (CPL R$104) em
   testes para Educação Financeira.
3. **Revisar se os 3 conjuntos com 0 leads** sofrem do mesmo bug de tracking corrigido em
   [[Diagnóstico e Plano de Ação - Liderança (ID Singular)]] — se sim, o CPL real de Educação
   Corporativa pode ser ainda melhor do que os R$233,85 calculados aqui (zero leads registrados não
   necessariamente é zero leads reais).

---
🔗 Relacionado: [[Acompanhamento - ID Singular]] · [[Histórico Meta 2025 - ID Singular]] · [[Backlog - Gestor de Tráfego Anterior (ID Singular)]] · [[Diagnóstico e Plano de Ação - Liderança (ID Singular)]]

#historico #meta-ads #educacao-corporativa #performance
