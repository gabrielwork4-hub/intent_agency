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

## 🧱 Estrutura (SEO + AEO)
- Title/H1: 
- Meta description: 
- Headings (H2/H3) + perguntas (PAA): 
- Pontos citáveis (GEO): 
- FAQ / schema: 

## 🔗 Links internos (cluster)
- 

## 🗣️ Tom de voz e CTA
- Tom (do cliente): 
- CTA / canal de conversão: 

#brief #conteudo
