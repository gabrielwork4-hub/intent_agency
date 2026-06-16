<%*
const cliente = await tp.system.prompt("Nome do cliente");
const cluster = await tp.system.prompt("Nome do cluster (ex: Bolos de Casamento)");
await tp.file.rename("Cluster - " + cluster + " (" + cliente + ")");
-%>
---
tipo: cluster-keywords
cliente: "[[<% cliente %>]]"
cluster: <% cluster %>
destino: 
prioridade: 
intencao: 
status: a fazer
atualizado: <% tp.date.now("YYYY-MM-DD") %>
tags: [keywords, cluster]
---

# 🔑 Cluster — <% cluster %> (<% cliente %>)

> Cluster de palavras-chave (Metodologia [[Metodologia - Estudo de Palavras-chave e Clusterização]]).
> Modelo serviço + pauta amarrados. Validado via Ahrefs/GSC.

## Keyword principal
- 

## Keywords secundárias
| Keyword | Volume | KD | Intenção | Destino (serviço/pauta) |
|---|---|---|---|---|
|  |  |  |  |  |

## Amarração (serviço ↔ pautas)
- Página de serviço: 
- Pautas de apoio: 

## Observações
- 

#keywords #cluster
