<%*
// Pergunta o nome do cliente e renomeia a nota automaticamente
const nome = await tp.system.prompt("Nome do cliente");
await tp.file.rename(nome);
-%>
---
tipo: cliente
nome: <% nome %>
segmento: 
status: ativo
vinculo: 
responsavel: Gabriel
funcao: estratégia
foco: 
inicio_contrato: 
site: 
instagram: 
telefone: 
endereco: 
atualizado: <% tp.date.now("YYYY-MM-DD") %>
tags: [cliente]
---

# <% nome %>

> Resumo do cliente em 1-2 linhas. Público em [[ICP - <% nome %>]] ·
> estratégia em [[Projeto - <% nome %>]].

## O que vende / faz
- 

## Onde atua
- 

## Canais de venda / conversão
- 

## Diferenciais
- 

## 🗣️ Tom de voz da marca
- 

## Inteligência do cliente
- 🎯 Público-alvo: [[ICP - <% nome %>]]
- 📈 Estratégia: [[Projeto - <% nome %>]]
- 📊 Acompanhamento e resultados: [[Acompanhamento - <% nome %>]]

## Anotações
- 

#cliente/ativo
