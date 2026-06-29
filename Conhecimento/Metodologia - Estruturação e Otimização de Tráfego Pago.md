---
tipo: metodologia
etapa: 9
fase: geração de demanda (mídia paga)
status: pronta
atualizado: 2026-06-29
tags: [metodologia, trafego-pago, tracking, budget, otimizacao, conhecimento]
---

# Metodologia - Estruturação e Otimização de Tráfego Pago

> **Objetivo:** servir como o "especialista em tráfego pago" consultado antes de qualquer decisão de
> budget, canal ou estrutura de campanha — cross-cliente, complementa
> [[Metodologia - Geração de Demanda - Google Ads]] e [[Metodologia - Geração de Demanda - Meta Ads]].
> Nasceu da auditoria real feita na ID Singular (29/06/2026): pixel instalado mas sem evento de
> conversão, conversão personalizada com regra impossível de bater, e budget sem critério de divisão
> por canal — três falhas comuns que essa metodologia existe para prevenir/diagnosticar.

## 🚦 Ordem de execução (nunca pular etapas)
1. **Auditoria de tracking** (sempre primeiro — antes de qualquer decisão de budget)
2. **Diagnóstico de dados históricos** (CPL real por canal, não só blended)
3. **Decisão de modelo** (sequencial vs. paralelo, conforme verba disponível)
4. **Divisão de budget** (entre frentes → entre canais)
5. **Configuração de otimização** (evento de conversão correto no nível certo)
6. **Ciclo de revisão** (fase de aprendizado, realocação por performance)

---

## 1️⃣ Auditoria de tracking (checklist obrigatório antes de validar qualquer dado)
Pixel instalado ≠ tracking funcionando. Validar nessa ordem:
- [ ] **O pixel carrega na página?** (testar via inspeção de rede/console, não só "ver o código no
  site") — confirma só que o `PageView` dispara, nada mais.
- [ ] **O evento de conversão dispara no envio real do formulário?** Testar com um envio de teste
  (dado marcado como "TESTE — NÃO CONTATAR", com permissão explícita do cliente) e observar a rede.
  - ⚠️ Formulários multi-etapa em SPA **não mudam de URL** — gatilhos baseados em "Page View numa
    URL de confirmação" não funcionam. Usar gatilho de clique (`Click Text`, não `Click ID` — botões
    novos raramente têm `id` fixo no HTML) ou evento customizado via `dataLayer.push`.
- [ ] **O evento chega no destino certo?** Verificar no Gerenciador de Eventos (Meta) / Tag Assistant
  (Google) — não confiar só no debug do GTM, confirmar em produção depois de publicar.
- [ ] **A campanha está otimizando pelo evento certo?** Conversões Personalizadas (Meta) podem ter
  regras de URL/texto que nunca batem — sempre inspecionar a regra exata, não só o nome.
- [ ] **UTMs chegam até o CRM?** Sem isso, o funil "canal → lead → SQL" quebra mesmo com pixel ok.

> **Regra de ouro:** nunca confiar em "0 resultados" como prova de que a campanha não está gerando
> leads — primeiro descartar quebra de tracking. Cruzar com o CRM/fonte de verdade real.

## 2️⃣ Diagnóstico de dados históricos
- Sempre buscar o **CPL por canal isolado**, não só o blended — um canal ineficiente pode estar
  escondendo um canal ótimo na média (ex.: ID Singular: blended R$555 vs. Meta isolado R$233,85).
- Identificar o **melhor conjunto/público/criativo histórico** (benchmark interno) antes de criar
  campanhas novas — replicar o que já funcionou em vez de começar do zero.
- Marcar conjuntos com **0 resultados e gasto relevante** como suspeitos de quebra de tracking, não
  como "público que não funciona" — investigar antes de descartar.

## 3️⃣ Decisão de modelo: sequencial vs. paralelo
| Cenário | Modelo recomendado |
|---|---|
| Verba fixa pequena (ex.: R$9k/mês), múltiplas frentes possíveis | **Sequencial** (1 frente por vez) evita diluição — mas trava o calendário de mercado |
| Frentes com histórico validado (CPL conhecido) + verba para sustentar 2-3 frentes com volume mínimo | **Paralelo**, com a frente mais validada recebendo a maior fatia |
| Frente nova sem dados | Entra com fatia pequena de teste, nunca empata em peso com frentes validadas |
| Lançamento sem material pronto | Não recebe budget — fatia fica reservada/redistribuída até material existir |

## 4️⃣ Divisão de budget — frentes → canais
**Entre frentes:** proporcional à validação (dado real > intuição). Frente recém-corrigida (tracking)
mantém prioridade até gerar dado limpo — não cortar verba no mesmo momento em que se corrige o
tracking (perde-se a leitura do "antes vs. depois").

**Entre canais (dentro de cada frente):** observado nos casos reais (ID Singular, ambas as frentes):
- **Meta Ads:** historicamente o canal de menor CPL no mix B2B testado — tende a receber a maior
  fatia (~70-80%) quando não há dado em contrário.
- **Google Ads:** menor volume, maior intenção — fatia menor (~10-15%), mas não cortar (captura
  demanda que já está procurando ativamente).
- **LinkedIn Ads:** segmentação por cargo é o diferencial — vale quando o público é claramente B2B
  por função (RH, CHRO, Diretoria); evitar usá-lo em mais de uma frente simultânea para o mesmo
  público (dilui sem necessidade).

## 5️⃣ Configuração de otimização
- **Sempre confirmar o nível onde o evento de conversão é selecionado** — em alguns canais
  (ex.: Meta), **não é editável após o conjunto de anúncios publicado**; a correção exige duplicar o
  conjunto, nunca editar o original.
- **Conversões personalizadas com regra de URL/texto são frágeis** — preferir evento padrão direto
  quando disponível e validado (ex.: "Lead") em vez de manter uma camada de conversão personalizada
  sem necessidade.
- Ao trocar o evento de otimização, **a fase de aprendizado reinicia** — é esperado (~3-7 dias para
  estabilizar), não é motivo para reverter a mudança no curto prazo.

## 6️⃣ Ciclo de revisão
- Validar em produção (não só em modo debug/preview) que o evento de conversão está sendo recebido
  com qualidade (Gerenciador de Eventos → score de correspondência).
- Comparar CPL real pós-correção contra o histórico — só then redistribuir budget entre canais/frentes
  com confiança.
- Registrar todo achado (causa raiz, correção, resultado) no Acompanhamento do cliente — vira
  histórico para a próxima auditoria.

---

## 📦 Entregável
Checklist de auditoria de tracking preenchido + diagnóstico de CPL por canal + proposta de divisão de
budget (frentes × canais) com justificativa baseada em dado real, não intuição.

## ✅ Critérios de qualidade
- Nenhuma decisão de budget tomada sem primeiro confirmar tracking funcionando.
- Toda divisão de canal/frente tem uma frase de "por quê" ancorada em dado (histórico ou validado).
- Toda correção de tracking é testada em produção antes de ser considerada resolvida (debug mode não
  é suficiente — confirmar visão geral/gerenciador de eventos real).

## 🚧 Backlog de evolução desta metodologia
- [ ] Mapear o equivalente de "Conversões Personalizadas frágeis" para Google Ads e LinkedIn Ads
  (esse caso foi documentado só para Meta até agora)
- [ ] Padronizar um teste de tracking pré-go-live como etapa obrigatória do checklist de lançamento
  (conectar com [[Metodologia - Geração de Demanda - Meta Ads]] e [[Metodologia - Geração de Demanda - Google Ads]])
- [ ] Definir gatilho/critério objetivo para "quando duplicar conjunto de anúncios" vs. "quando criar
  campanha nova do zero"

---
🔗 Relacionado: [[📚 Conhecimento]] · [[Metodologia - Geração de Demanda - Meta Ads]] · [[Metodologia - Geração de Demanda - Google Ads]] · anterior → [[Metodologia - Geração de Demanda - Meta Ads]]

#metodologia #trafego-pago #tracking #budget
