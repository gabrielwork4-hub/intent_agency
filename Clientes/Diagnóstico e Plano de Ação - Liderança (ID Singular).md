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

### 🔴 Causa raiz confirmada (teste em 21/06 via navegador) — vale para os DOIS funis
⚠️ **Metade dos criativos da campanha aponta para `/diagnostico-lideranca` e a outra metade para
`/lideranca`** — são dois funis de conversão diferentes, e o problema afeta os dois:
- `/diagnostico-lideranca`: quiz de 4 etapas de cadastro + 10 perguntas. Lead de teste "TESTE NAO
  CONTATAR — QA Pixel" enviado (a excluir do CRM Wevia).
- `/lideranca`: formulário de qualificação de **11 etapas** ("Quero traçar uma jornada de liderança
  sob medida"), que **notifica o time comercial** ("em breve nossa equipe vai te chamar"). Lead de
  teste "TESTE NAO CONTATAR QA" / "QA Pixel" enviado em 21/06 — **avisar o time comercial para
  ignorar esse contato** e excluir do CRM Wevia.
- ✅ Achado positivo: o formulário de `/lideranca` já tem campos ocultos de UTM prontos
  (`utm_source`, `utm_medium`, `utm_campaign`, `utm_content`, `utm_term`, `origem`, `lp`,
  `conversion_identifier`) — só precisam vir preenchidos a partir da URL do anúncio (ver padrão de
  UTM acima). O quiz não tem esses campos visíveis.

Testei o fluxo completo do formulário em `/diagnostico-lideranca` (4 etapas, lead de teste marcado
"TESTE NAO CONTATAR — QA Pixel", **a excluir do CRM Wevia**):
- GTM (`GTM-NS38H4VJ`, mesmo container nas duas páginas) dispara `gtm.formSubmit`/`form_submit` em
  **todas as etapas dos dois formulários** — já conectado a uma tag do **Google Ads** (confirmado nos
  dois funis).
- Pixel do Meta (`488385575868107`, mesmo pixel nas duas páginas) dispara `PageView` normalmente, mas
  **não dispara nenhum evento de conversão (Lead/CompleteRegistration) em nenhuma etapa de nenhum dos
  dois formulários** — confirmado com envio completo e bem-sucedido nos dois (quiz abriu; "Recebemos o
  seu contato" apareceu no formulário de 11 etapas).
- **Causa raiz:** falta a tag de Meta Pixel conectada ao envio de QUALQUER formulário no GTM. O Meta
  nunca recebe sinal de conversão → 0 resultados no relatório nos dois funis, mesmo com leads reais
  entrando → algoritmo do Meta otimiza sem feedback nenhum, em 100% do orçamento de Meta Ads.

**Correção recomendada:**
1. Pedir ao dev um evento customizado no código (ex.: `dataLayer.push({event:'diagnostico_lead_enviado'})`
   e `dataLayer.push({event:'lideranca_form_enviado'})`) disparado só na confirmação final de cada
   formulário — **não** usar o trigger genérico "Form Submission" do GTM (dispara em todas as etapas,
   geraria Lead duplicado várias vezes por pessoa).
2. Criar tag "Meta Pixel - Lead" no GTM (`fbq('track','Lead')`) usando esses eventos customizados como
   trigger — uma tag pode ter múltiplos triggers (um por funil) ou criar duas tags espelhadas.
3. Publicar o container.
4. Médio prazo: migrar para **Meta Conversions API** (servidor→servidor, a partir do Wevia) — mais
   robusto que pixel client-side contra ad-blocker/Safari ITP, comum em tráfego corporativo/RH.

**Correção rápida sem dev (Element Visibility no GTM) — testada em 21/06:**
- `/diagnostico-lideranca`: trigger de Visibilidade do Elemento, seletor CSS `.sticky.top-20 p.tabular-nums`
  (texto "Pergunta 1 de 10" — só aparece após envio do cadastro), "uma vez por página".
- `/lideranca`: precisa de seletor equivalente para a tela de confirmação "Recebemos o seu contato."
  (não capturado ainda — pegar o seletor antes de configurar o trigger).
- ⚠️ Frágil: depende de classes Tailwind que podem mudar em deploys futuros sem aviso.

**Ação imediata adicional:** avisar o time comercial que recebe notificação do formulário de
`/lideranca` para **ignorar os contatos "TESTE NAO CONTATAR QA" / "QA Pixel"** gerados nesta validação.

### ✅ RESOLVIDO (29/06/2026)
Causa raiz real: o acionador `[FORM PRINCIPAL] CADASTRO` dependia de `Click ID contém
btn-educorp-enviar-lv1` — um ID de botão que só existe no formulário antigo (`/educacao-corporativa`).
Os botões novos (quiz e `/lideranca`) não têm `id`, só classes Tailwind genéricas, então o acionador
nunca disparava para Google, LinkedIn **nem** Meta nesses dois funis.

**Correção aplicada no GTM (`GTM-NS38H4VJ`), Versão 4:**
- Habilitada a variável incorporada `Click Text`.
- Criados 2 acionadores novos: `[FORM QUIZ LIDERANÇA] CADASTRO` (`Click Text` = `Iniciar Diagnóstico`)
  e `[FORM LIDERANÇA] CADASTRO` (`Click Text` contém `Enviar` E `Page Path` contém `/lideranca`).
- Acionadores adicionados às 3 tags existentes: `[GOOGLE]`, `[LINKEDIN]`, `[META] CADASTRO LEAD
  (FORM PRINCIPAL)` — resolve os 3 canais de uma vez, sem precisar de dev.
- **Confirmado no debug nativo do GTM:** as 3 tags disparam corretamente ("Disparou 1 vez" cada) no
  envio do quiz de `/diagnostico-lideranca`.
- Leads de teste gerados durante a validação ("TESTE NAO CONTATAR" / "QA Pixel" / variações) — **a
  excluir do CRM Wevia**, e avisar o time comercial sobre o contato de teste de `/lideranca`.

**Confirmado em produção (29/06, Gerenciador de Eventos do Meta):** evento **Lead** ativo, 12 eventos
recebidos, qualidade 8.7/10, 100% de correspondência avançada via Conversions API (pixel
`488385575868107`, conjunto "[EDUCAÇÃO CORPORATIVA]"). Correção 100% validada de ponta a ponta.

**Pendência seguinte:** verificar o "Objetivo de desempenho" dos conjuntos de anúncios ativos no
Gerenciador de Anúncios — como o evento Lead não existia até agora, é provável que estejam otimizando
por "Cliques no link"/"Visualizações da LP" em vez de "Lead". Trocar para Lead reinicia a fase de
aprendizado (esperado, ~3-7 dias para estabilizar), mas faz o algoritmo entregar pra quem converte,
não só pra quem clica.

### 🔴→✅ Segunda causa raiz encontrada e corrigida (29/06/2026)
Os conjuntos de anúncios estavam otimizando por uma **Conversão Personalizada quebrada**, chamada
"Iniciar Diagnóstico" (ID 1634960754277864) — regra: `URL contém "Iniciar Diagnóstico"`, que nunca
poderia disparar (é o texto do botão, não da URL da página). Por isso o Meta nunca contabilizava
resultado, mesmo com o pixel/GTM já corrigidos e o evento Lead chegando (confirmado 12 eventos,
qualidade 8.7/10 no Gerenciador de Eventos).

**Correção:** Meta não permite editar evento de conversão de conjunto já publicado, nem editar regra
de conversão personalizada já criada. Solução: criada uma conversão personalizada nova e correta —
**"Lead - Diagnóstico Liderança"** (Evento: Lead · Regra: URL contém "idsingular.com.br") — e os 2
conjuntos de anúncios ativos (`01 - [LP Liderança] Quente + Lookalike` e `02 - [LP Liderança]
Prospecção Fria`) foram **duplicados** apontando para essa conversão nova. Conjuntos originais
(quebrados) devem ser pausados após confirmar que as cópias estão ativas.
**Efeito esperado:** fase de aprendizado reinicia nos novos conjuntos (~3-7 dias para estabilizar),
mas a partir de agora o algoritmo otimiza por quem realmente converte, não só por clique.

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
