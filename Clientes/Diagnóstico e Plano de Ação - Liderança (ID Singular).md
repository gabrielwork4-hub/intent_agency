---
tipo: diagnostico-plano-acao
cliente: "[[ID Singular]]"
lancamento: Liderança · 23/06–22/07/2026
atualizado: 2026-06-16
tags: [diagnostico, plano-de-acao, lideranca, id-singular]
---

# 🩺 Diagnóstico e Plano de Ação — Liderança (ID Singular)

> Diagnóstico da situação + plano de ação até o go-live (23/06) e durante o sprint (23/06–22/07).
> Visão geral em [[Overview do Lançamento - Liderança (ID Singular)]].

---

## 🩺 DIAGNÓSTICO

### Situação atual (histórico fev–mai/2026)
52 leads · 6 SQLs · 1 fechamento · investimento R$ 28.877 · **CPL R$ 555** · custo/SQL R$ 4,8 mil ·
conversão lead→SQL 11,53% · **ROI 120%** (só educação corporativa).
> Há resultado e ROI positivo, mas a **eficiência de aquisição é cara** (CPL alto).

### 🔴 Problemas identificados
0. ~~**⛔ BLOQUEADOR — contas de anúncio paradas**~~ → ✅ **RESOLVIDO (17/06):** Meta e LinkedIn
   regularizadas/pagas. Go-live liberado. Ver [[Backlog - Gestor de Tráfego Anterior (ID Singular)]].
1. **CPL alto (R$ 555)** — a meta de R$ 182 exige eficiência ~3x maior.
2. **LP pública sem formulário** — a /educacao-corporativa leva a WhatsApp/e-mail. *(Obs.: a captura
   por formulário JÁ existia via instant form + CRM "Jornada Educação Corporativa" — o gap é a LP
   pública, não a ausência total de captura.)*
3. **LP genérica** — sem oferta de conversão e **sem os diferenciais** (Metodologia Singular®,
   mensuração emocional) que vencem a concorrência.
4. **Funil incompleto** — MQL não estava definido.
5. **Baixa demanda de busca** — liderança tem pouco volume no Google → não sustenta volume sozinho.
6. ~~Sprint curto~~ → ✅ **resolvido:** roda **30 dias** (aprendizado amortiza + tempo de otimizar).

### 🟢 Oportunidades
1. **Oceano azul de posicionamento** — ninguém ocupa "humanização + método + performance".
2. **Prova social forte e subutilizada** — Petrobras, Mercedes, Caixa, Unimed, Sicredi, Metrô SP...
3. **Base de maio (+1.000)** — pronta para remarketing/lookalike (converte rápido).
4. **Oferta de diagnóstico** — alto valor percebido, baixo atrito → destrava o lead qualificado.

### ⚠️ Risco principal
Meta otimista (CPL R$ 182) é teto, não promessa. **Recomendação:** base de trabalho = **~30 leads /
~3–4 SQLs / CPL ~R$ 300** (30 dias diretos — ver [[Projeção 30 Dias - Liderança (ID Singular)]]).
Rodar 30 dias (não sprint) reduz o risco: a fase de aprendizado amortiza e há tempo de otimizar.

---

## ✅ PLANO DE AÇÃO

### Fase 1 — Pré-lançamento (até 21/06)
| # | Ação | Responsável | Prazo | Status |
|---|---|---|---|---|
| 0 | ✅ ~~Regularizar conta Meta e LinkedIn~~ — **FEITO (17/06)** | Cliente | concluído | ✅ |
| 1 | ✅ ~~Aprovar copy da LP e dos anúncios~~ — **FEITO (21/06)** | Cliente | 19/06 | ✅ |
| 2 | ✅ ~~Liberar logos/cases / criativos~~ — **criativos prontos (21/06)** | Cliente | 19/06 | ✅ |
| 3 | ✅ ~~LP validada~~ — falta confirmar GA4 + pixel instalados na LP | Time/cliente | 21/06 | ⚠️ parcial |
| 4 | Definir MQL + configurar **eventos de conversão e UTMs** | Nós + time | 20/06 | 🔴 **em aberto — ver padrão de UTM abaixo** |
| 5 | Montar campanhas (Meta/Google/LinkedIn) com a copy | Mídia | 21/06 | ⏳ a confirmar |
| 6 | Conferir públicos: remarketing (base de maio) + lookalike | Mídia | 21/06 | ⏳ a confirmar |

### 🔗 Padrão de UTMs — Liderança (ID Singular)
> Necessário para saber **qual canal/anúncio gerou cada lead** no GA4 e no CRM Wevia (que recebe os
> envios do [[Quiz - Diagnóstico de Liderança (ID Singular)]]). Sem UTM, todo lead cai como "direto/orgânico"
> e perdemos a leitura de CPL por canal — que é a métrica central de todo o [[Plano de Mídia - Liderança (ID Singular)]].

**Estrutura padrão (todo link de anúncio deve ter os 5 parâmetros):**
```
?utm_source=[canal]&utm_medium=[tipo]&utm_campaign=lideranca_jun26&utm_content=[anuncio]&utm_term=[publico]
```

| Parâmetro | O que identifica | Valores para esta campanha |
|---|---|---|
| `utm_source` | Onde o clique aconteceu | `meta`, `google`, `linkedin` |
| `utm_medium` | Tipo de mídia | `cpc` (pago) — usar `social` só se for orgânico |
| `utm_campaign` | Nome da campanha (fixo) | `lideranca_jun26` |
| `utm_content` | Qual anúncio/criativo | `anuncio1`, `anuncio2`, `anuncio3`, `anuncio4` (ver [[Anúncios - Liderança (ID Singular)]]) |
| `utm_term` | Qual público | `remarketing`, `lookalike`, `frio` |

**Exemplos prontos para colar no destino dos anúncios:**
- Meta (remarketing, anúncio 4): `idsingular.com.br/diagnostico-lideranca?utm_source=meta&utm_medium=cpc&utm_campaign=lideranca_jun26&utm_content=anuncio4&utm_term=remarketing`
- Google (público frio): `idsingular.com.br/diagnostico-lideranca?utm_source=google&utm_medium=cpc&utm_campaign=lideranca_jun26&utm_term=frio`
- LinkedIn: `idsingular.com.br/diagnostico-lideranca?utm_source=linkedin&utm_medium=cpc&utm_campaign=lideranca_jun26`

**Como funciona na prática:**
1. Cada plataforma de anúncio (Meta Ads Manager, Google Ads, LinkedIn Campaign Manager) tem um campo
   "URL de destino" por anúncio — é ali que entra o link completo com UTM, não na URL genérica da LP.
2. O GA4 lê esses parâmetros automaticamente e separa o tráfego por `Source/Medium/Campaign` nos
   relatórios de aquisição — não precisa configurar nada extra no GA4 além do pixel/tag estar instalado.
3. Como o formulário do quiz salva no **CRM Wevia**, o ideal é confirmar com o time técnico se a página
   carrega a UTM da URL e a **anexa ao registro do lead** (campo oculto no formulário) — isso é o elo que
   falta para ligar "lead no CRM" a "anúncio que gerou esse lead". **Sem esse campo oculto, o GA4 mostra
   o canal, mas o CRM não sabe qual anúncio converteu** — pior cenário para calcular CPL/SQL por criativo.
4. `utm_campaign` deve ser **sempre o mesmo valor** (`lideranca_jun26`) em todos os canais — é o que
   permite somar todo o investimento da campanha num único relatório.

**Pendência a confirmar com o time técnico:** o formulário do quiz grava a UTM de origem (campo oculto)
junto com o lead no CRM Wevia? Se não, é o ajuste técnico mais urgente antes do go-live.

### Fase 2 — Go-live e sprint (23/06–22/07)
| #   | Ação                                                            | Responsável | Quando             |
| --- | --------------------------------------------------------------- | ----------- | ------------------ |
| 7   | Subir campanhas; **priorizar remarketing/lookalike** no início  | Mídia       | 23/06              |
| 8   | Subir primeiro os criativos de maior conversão (Anúncios 4 e 2) | Mídia       | 23/06              |
| 9   | Monitorar CPL/leads **diariamente**; ajustar lances/criativos   | Mídia       | 23/06–22/07           |
| 10  | **Realocar verba** para o canal de melhor CPL/SQL               | Mídia       | a partir de ~25/06 |
| 11  | Pausar anúncio com CPL > 1,5× a média; escalar o melhor         | Mídia       | contínuo           |

### Fase 3 — Pós-sprint (a partir de 01/07)
| #   | Ação                                                                      | Responsável   | Quando |
| --- | ------------------------------------------------------------------------- | ------------- | ------ |
| 12  | Consolidar resultados (leads, CPL, SQLs por canal)                        | Nós           | 01/07  |
| 13  | Registrar aprendizados em [[Aprendizados Validados]]                      | Nós           | 01/07  |
| 14  | Refinar anti-ICP com dados de qualificação/fechamento                     | Nós + cliente | 01/07  |
| 15  | Decidir continuidade/escala e preparar lançamento 2 (Comunicação · 06/07) | Nós           | 01/07  |

## 📊 Como saberemos que deu certo
Meta semanal: ~7 leads · ~1 SQL (30 dias). Acompanhamento em [[Acompanhamento - ID Singular]].
Sucesso = **~30 leads / ~3–4 SQLs** com CPL ~R$ 300 (bem abaixo do histórico R$ 555).

---
🔗 Relacionado: [[Overview do Lançamento - Liderança (ID Singular)]] · [[Plano de Mídia - Liderança (ID Singular)]] · [[Estrutura de Campanha - Liderança (ID Singular)]]

#diagnostico #plano-de-acao #lideranca
