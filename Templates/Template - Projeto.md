<%*
const nome = await tp.system.prompt("Nome do cliente");
const titulo = await tp.system.prompt("Título do projeto (ex: SEO, Geração de Demanda)");
await tp.file.rename("Projeto - " + titulo + " " + nome);
-%>
---
tipo: projeto
cliente: "[[<% nome %>]]"
vinculo: 
foco: <% titulo %>
status: em início
prioridade: alta
prazo: 
atualizado: <% tp.date.now("YYYY-MM-DD") %>
tags: [projeto]
---

# 📈 Projeto — <% titulo %> <% nome %>

> Estratégia do projeto. Público em [[ICP - <% nome %>]].

## 🎯 Objetivos
- 

## 🔑 Palavras-chave / foco
- 

## 🛠️ Frentes de trabalho
- [ ] 

## 📊 Métricas
- 

## ✅ Próximos passos
- [ ] 

---
🔗 Relacionado: [[<% nome %>]] · [[Acompanhamento - <% nome %>]]

#projeto
