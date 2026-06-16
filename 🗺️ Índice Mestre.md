---
tipo: indice-mestre
papel: ponto de entrada do cofre
atualizado: 2026-06-15
tags: [moc, indice]
---

# 🗺️ Índice Mestre

> **Ponto de entrada do cofre.** Esta é a base de inteligência dos clientes em que atuo.
> Quem chega aqui (humano ou IA) começa por esta nota para saber onde está cada coisa.
> Para a IA: ver também [[🤖 Manual do Cofre para IA]] e [[00 - Guia e Convenções do Cofre]].

## 👥 Clientes
Base de inteligência por cliente.

### Agência — Intent Marketing
- [[Mari Quitutes]] — confeitaria · *ativo*
  - [[ICP - Mari Quitutes]] — público-alvo
  - [[Projeto - SEO Mari Quitutes]] — estratégia de SEO
- [[Gold Car]] — mecânica automotiva · *ativo*
  - [[ICP - Gold Car]] — público-alvo
  - [[Projeto - SEO Gold Car]] — estratégia de SEO

### PJ — fora da Intent Marketing
- [[ID Singular]] — consultoria / educação corporativa · *em início*
  - [[ICP - ID Singular]] — público-alvo
  - [[Escopo - ID Singular]] — o que ela vende
  - [[Projeto - Geração de Demanda ID Singular]] — estratégia

> Índice detalhado de clientes em [[👥 Clientes]].

## 📚 Conhecimento
Metodologias, checklists e referências reutilizáveis.
- [[📚 Conhecimento]] — índice da base de conhecimento e metodologias

## 📐 Estrutura e padrões
- [[00 - Guia e Convenções do Cofre]] — como nomear, estruturar e padronizar notas
- [[🤖 Manual do Cofre para IA]] — orientação para o Claude consultar o cofre
- [[🚀 Roadmap de Evolução do Cofre]] — plano de melhorias e inovações por fase
- [[📋 Templates]] — modelos padronizados de nota (Templater)

## 🧪 Exemplos (aprendizado — pode apagar)
- [[🏠 Painel Central]] · [[📊 Painel Dataview]]

---

## 📊 Visão automática dos clientes (requer Dataview)
```dataview
TABLE segmento, status, vinculo, funcao AS "Função"
FROM "Clientes"
WHERE tipo = "cliente"
SORT status ASC
```

#moc #indice
