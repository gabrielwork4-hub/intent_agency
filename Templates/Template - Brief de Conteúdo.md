<%*
const cliente = await tp.system.prompt("Nome do cliente");
const titulo = await tp.system.prompt("Título da peça (ex: Bolos de Casamento)");
await tp.file.rename("Brief - " + titulo);
-%>
---
tipo: brief-conteudo
cliente: "[[<% cliente %>]]"
peca: <% titulo %>
destino: 
status: a fazer
ymyl: não
commodity: 
atualizado: <% tp.date.now("YYYY-MM-DD") %>
tags: [brief, conteudo]
---

# 📝 Brief — <% titulo %>

> Segue [[Metodologia - Brief para Produção de Artigos e Páginas]] (SEO + AEO + GEO).
> Produção por Claude + conectores; este brief padroniza o que rankeia.
> Cliente: [[<% cliente %>]]

## 🔬 Benchmark de SERP
- Quem rankeia / padrões replicáveis: 

## 🎯 Cluster e destino
- Cluster/tópico: 
- Destino: serviço ☐ / pauta ☐ — amarração: 

## 🔑 Keyword e intenção
- Principal: 
- Secundárias: 
- Intenção: 

## 🏷️ Classificação
- YMYL: sim ☐ / não ☐ — se sim, reforçar E-E-A-T/fontes
- Commodity: ângulo diferenciador → 

## 🧱 Estrutura (SEO + AEO) — hierarquia H1 > H2 > H3 > H4
> Headings = leitura para os motores (Google fatia o tema; LLMs fatiam em chunks por heading).
> Usar H3/H4 quando necessário; um só H1; não pular níveis; heading espelha a pergunta real.
- Title/H1 (até 65 caracteres): 
- Meta description (até 165 caracteres): 
- Headings (H2 = tópicos; H3/H4 = subtópicos) + perguntas (PAA): 
- Pontos citáveis (GEO): 
- FAQ / schema: 

## 🔗 Links internos (cluster)
- 

## 🗣️ Tom de voz e CTA
- Tom (do cliente): 
- CTA / canal de conversão: 

#brief #conteudo
