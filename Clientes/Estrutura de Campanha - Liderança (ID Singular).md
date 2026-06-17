---
tipo: estrutura-campanha
cliente: "[[ID Singular]]"
lancamento: Liderança · 22/06/2026
budget: R$ 9.000
atualizado: 2026-06-16
tags: [estrutura-campanha, performance, lideranca, id-singular]
---

# ⚙️ Estrutura de Campanha — Liderança (blueprint de setup)

> Blueprint operacional para subir as campanhas. Segue [[Plano de Mídia - Liderança (ID Singular)]]
> (verba) e [[Anúncios - Liderança (ID Singular)]] (copy). Destino: [[Copy LP - Diagnóstico de Liderança (ID Singular)]].

## ⏱️ Janela e pacing do budget
- **Rodando apenas de 22/06 a 30/06 (9 dias).** R$ 9.000 concentrados → **~R$ 1.000/dia**.
- Split por canal (no total): Meta R$ 5.500 · Google R$ 2.000 · LinkedIn R$ 1.500.
  - Diário aprox. (9 dias): **Meta ~R$ 610 · Google ~R$ 220 · LinkedIn ~R$ 165**.
- **Previsibilidade (por CPL):** R$ 9k ÷ R$ 182 ≈ 49–52 leads · ~6 SQLs.

> ⚠️ **Implicações do sprint de 9 dias (sem aquecimento):**
> 1. **Fase de aprendizado** das campanhas consome os primeiros ~2–3 dias → CPL inicial mais alto.
> 2. Sem warm-up, **priorizar públicos quentes desde o dia 22**: remarketing da base de maio (+1.000)
>    e lookalike convertem mais rápido que prospecção fria.
> 3. Janela curta + aprendizado → **cenário conservador (R$ ~210 CPL / ~43 leads) é o mais provável**;
>    a meta cheia (52) é o teto. Alinhar essa expectativa com o cliente.
> 4. Concentrar criativos de **maior conversão** logo no início (Anúncios 4-remarketing e 2-CHRO).

## 🏷️ Convenção de nomes
`IDS_Lideranca_[Canal]_[Objetivo]_[Publico]_jun26`
Ex.: `IDS_Lideranca_Meta_Leads_Lookalike_jun26`

---

## 📱 META ADS — R$ 5.500 (objetivo: Cadastros/Leads)
### Campanha 1 — Prospecção (R$ 3.500)
- **Conjunto A — Lookalike:** 1–3% de leads/clientes e da base de maio. Ads: 1 (Gestor) + 3 (autoridade).
- **Conjunto B — Interesse/cargo:** RH, gestão de pessoas, T&D, desenvolvimento organizacional;
  30–55 anos; Brasil (priorizar regiões dos clientes). Ads: 1 (Gestor) + 3 (autoridade).
### Campanha 2 — Remarketing (R$ 2.000)
- **Conjunto único:** visitantes do site (90d) + **base de maio (+1.000)** + engajados FB/IG.
  Ads: 4 (remarketing) + 2 (CHRO/dados).
- **Posicionamentos:** Advantage+ (feed/stories/reels). **Otimização:** por conversão (lead na LP).

## 🔎 GOOGLE SEARCH — R$ 2.000 (objetivo: Conversões/Leads)
- **1 campanha "Liderança – alta intenção"** · Rede de Pesquisa apenas (sem Display/PMax).
- **Grupos de anúncio por tema:** (a) "programa/treinamento de liderança"; (b) "desenvolvimento de
  líderes/lideranças"; (c) "consultoria/formação de líderes".
- **RSA:** títulos e descrições de [[Anúncios - Liderança (ID Singular)]]. **Negativas** aplicadas.
- **Lance:** Maximizar conversões (ou tCPA após dados). Cap por volume baixo de busca.

## 💼 LINKEDIN — R$ 1.500 (teste · objetivo: Lead Gen)
- **1 campanha** · Lead Gen Form nativo.
- **Segmentação:** cargos (CHRO, Dir./Ger. RH, DHO, T&D) · porte 201+ · setores ICP.
- Copy/campos de [[Anúncios - Liderança (ID Singular)]].

---

## 🎯 Definição de funil (fechar o "?" de MQL)
- **Lead:** preencheu o formulário da LP.
- **MQL:** lead dentro do ICP (cargo de gestão/RH + porte ≥ alvo) — *qualificado pelos campos do form*.
- **SQL:** MQL que agendou/realizou o diagnóstico (intenção real).
- Meta: 52 leads → ~6 SQLs (manter conversão ≥ 11,53%).

## 📈 Rastreamento (pré-requisito)
- **Pixel Meta** + **Tag Google** + **GA4** com evento de conversão no envio do formulário.
- **UTMs** padronizadas por canal/conjunto/anúncio (medir CPL por origem).
- LinkedIn: conversão via Lead Gen Form (nativo) + Insight Tag.

## 🔧 Regras de otimização (semanal)
- Realocar verba para o canal/conjunto de **menor CPL com SQL** após 7–10 dias.
- Pausar anúncio com CPL > 1,5× a média; escalar o de melhor desempenho.
- Acompanhar em [[Acompanhamento - ID Singular]] (meta semanal: ~13 leads / ~1,5 SQL).

## ✅ Checklist de go-live (responsável)
- [ ] LP publicada com formulário + GA4 + pixel *(time/cliente)*
- [ ] Confirmar pacing do budget (mês x janela)
- [ ] Cases/logos liberados para anúncio
- [ ] UTMs e eventos de conversão configurados
- [ ] Campanhas montadas (Meta/Google/LinkedIn) com a copy aprovada

---
🔗 Relacionado: [[Plano de Mídia - Liderança (ID Singular)]] · [[Anúncios - Liderança (ID Singular)]] · [[Brief de Campanha - Liderança (ID Singular)]]

#estrutura-campanha #performance #lideranca
