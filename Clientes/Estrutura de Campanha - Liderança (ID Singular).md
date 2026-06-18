---
tipo: estrutura-campanha
cliente: "[[ID Singular]]"
lancamento: Liderança · 23/06/2026
budget: R$ 9.000
atualizado: 2026-06-16
tags: [estrutura-campanha, performance, lideranca, id-singular]
---

# ⚙️ Estrutura de Campanha — Liderança (blueprint de setup)

> Blueprint operacional para subir as campanhas. Segue [[Plano de Mídia - Liderança (ID Singular)]]
> (verba) e [[Anúncios - Liderança (ID Singular)]] (copy). Destino: [[Copy LP - Diagnóstico de Liderança (ID Singular)]].

## ⏱️ Janela e pacing do budget
- **Rodando 30 dias diretos** (início seg. 23/06 → ~22/07). R$ 9.000 → **~R$ 300/dia**.
- Split por canal: **Meta R$ 6.500 · LinkedIn R$ 1.500 · Google R$ 1.000** (ajustado p/ 30 dias —
  ver [[Projeção 30 Dias - Liderança (ID Singular)]]).
- **Pacing fasado:** aquecimento (dias 1–7, ~R$ 1.800) → otimização (8–21, ~R$ 4.200) →
  escala no vencedor (22–30, ~R$ 3.000).
- **Previsibilidade (real):** CPL efetivo ~R$ 300 → **~30 leads · ~3–4 SQLs** (custo/SQL ~R$ 2.500).

> ✅ **Vantagem dos 30 dias:** a fase de aprendizado amortiza, há ciclos de otimização e o
> remarketing amadurece → CPL menor que o sprint. LinkedIn em **janela focada (~2 semanas)**, não
> diário (R$ 300/dia é enxuto para 3 canais; concentrar no Meta).

## 🏷️ Convenção de nomes
`IDS_Lideranca_[Canal]_[Objetivo]_[Publico]_jun26`
Ex.: `IDS_Lideranca_Meta_Leads_Lookalike_jun26`

---

## 📱 META ADS — R$ 6.500 (objetivo: Cadastros/Leads)
### Campanha 1 — Remarketing + Lookalike (R$ 3.500) · converte primeiro
- **Conjunto Remarketing:** visitantes do site (90d) + **base de maio (+1.000)** + engajados FB/IG.
  Ads: 4 (remarketing) + 2 (CHRO/dados).
- **Conjunto Lookalike:** 1–3% de leads/clientes e da base de maio. Ads: 2 (CHRO) + 3 (autoridade).
### Campanha 2 — Prospecção fria (R$ 3.000)
- **Conjunto Interesse/cargo:** RH, gestão de pessoas, T&D, desenvolvimento organizacional,
  Leadership development; 30–55 anos; Brasil (priorizar regiões dos clientes). Ads: 1 (Gestor) + 3 (autoridade).
- **Posicionamentos:** Advantage+ (feed/stories/reels). **Otimização:** por conversão (lead na LP).
- 💡 **Funil 2 passos (do histórico 2025):** rodar posts de tráfego/engajamento baratos
  (~R$ 0,43/clique, temas gestão/transformação) para **encher a audiência de remarketing** →
  retargetar com a oferta do Diagnóstico. Audiência quente derruba o CPL. Ver [[Histórico Meta 2025 - ID Singular]].

## 🔎 GOOGLE SEARCH — R$ 1.000 (objetivo: Conversões/Leads)
- **1 campanha "Liderança – alta intenção"** · Rede de Pesquisa apenas (sem Display/PMax).
- **Grupos de anúncio por tema:** (a) "programa/treinamento de liderança"; (b) "desenvolvimento de
  líderes/lideranças"; (c) "consultoria/formação de líderes".
- **RSA:** títulos e descrições de [[Anúncios - Liderança (ID Singular)]]. **Negativas** aplicadas.
- **Lance:** Maximizar conversões (ou tCPA após dados). Cap por volume baixo de busca.

## 💼 LINKEDIN — R$ 1.500 (qualidade · burst ~2 semanas · objetivo: Lead Gen)
- **1 campanha** · Lead Gen Form nativo.
- **Segmentação:** cargos (CHRO, Dir./Ger. RH, DHO, T&D) · porte 201+ · setores ICP.
- Copy/campos de [[Anúncios - Liderança (ID Singular)]].

---

## 🎯 Definição de funil (fechar o "?" de MQL)
- **Lead:** preencheu o formulário da LP.
- **MQL:** lead dentro do ICP (cargo de gestão/RH + porte ≥ alvo) — *qualificado pelos campos do form*.
- **SQL:** MQL que agendou/realizou o diagnóstico (intenção real).
- Meta de trabalho: **~30 leads → ~3–4 SQLs** (teto otimista 52/6). Manter conversão ≥ 11,53%.

## 📈 Rastreamento (pré-requisito)
- **Pixel Meta** + **Tag Google** + **GA4** com evento de conversão no envio do formulário.
- **UTMs** padronizadas por canal/conjunto/anúncio (medir CPL por origem).
- LinkedIn: conversão via Lead Gen Form (nativo) + Insight Tag.

## 🔧 Regras de otimização (semanal)
- Realocar verba para o canal/conjunto de **menor CPL com SQL** após 7–10 dias.
- Pausar anúncio com CPL > 1,5× a média; escalar o de melhor desempenho.
- Acompanhar em [[Acompanhamento - ID Singular]] (meta semanal: ~7 leads / ~1 SQL).

## ✅ Checklist de go-live (responsável)
- [ ] LP publicada com formulário + GA4 + pixel *(time/cliente)*
- [ ] Confirmar pacing do budget (mês x janela)
- [ ] Cases/logos liberados para anúncio
- [ ] UTMs e eventos de conversão configurados
- [ ] Campanhas montadas (Meta/Google/LinkedIn) com a copy aprovada

---
🔗 Relacionado: [[Plano de Mídia - Liderança (ID Singular)]] · [[Anúncios - Liderança (ID Singular)]] · [[Brief de Campanha - Liderança (ID Singular)]]

#estrutura-campanha #performance #lideranca
