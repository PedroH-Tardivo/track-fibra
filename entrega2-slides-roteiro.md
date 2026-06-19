# Entrega 2 — Roteiro dos Slides (Track Fibra)

> Conteúdo aprovado dos 10 slides da apresentação (≤15 min). Estilo visual: **Sinal & Fibra** — navy `#0B1220`, azul `#1D4ED8`, ciano `#06B6D4`, geométrico com motivo de sinal.
> **Status:** a geração no Canva (IA) estava falhando no servidor (jun/2026) — roteiro guardado para regerar quando voltar, ou montar manualmente / via .pptx.
> Cobertura: itens 2.1 a 2.4 da Entrega 2. Slides 8 e 9 dependem da execução do teste (marcados **[A PREENCHER]**).

---

## 1 · Track Fibra (capa)
- Sistema de gerenciamento de chamadas de serviço para provedores de internet (web + mobile)
- Equipe: Kauan Silva Schiavon · Leonardo Hideki Gen Sato · Pedro Henrique Tardivo Rodrigues · Guilherme Fiuza R. P. de Carvalho
- UTFPR – Campo Mourão · Bacharelado em Ciência da Computação
- Interação Humano-Computador · 2026

## 2 · O problema *(2.1 — motivação)*
- O trabalho de campo é coordenado por planilha e WhatsApp, sem fonte única de informação
- Técnicos se deslocam à toa por dados incorretos ou incompletos
- Supervisores não têm visibilidade: cobram status o tempo todo pelo WhatsApp
- Dependência da memória e ausência de rota organizada

## 3 · Pré-sprint: o que motivou *(2.1)*
- 2 questionários (Google Forms), 17 respondentes: 12 técnicos + 5 supervisores (via provedor NetFibra)
- Falta de fonte única e confiável de informação
- Falta de visibilidade da operação
- Dependência da memória e ausência de rota foi o item pior avaliado
- Supervisores: 100% usam computador → confirma a versão web

## 4 · A solução: Track Fibra *(2.1)*
- Para o técnico: um organizador confiável do dia de trabalho (app mobile)
- Para o supervisor: uma central de visibilidade da operação (web)
- Dois perfis, um produto: duas pontas do mesmo fluxo
- Três tipos de chamada: instalação, manutenção e recolhimento

## 5 · Design Sprint: foco no técnico *(consistência de método)*
- Mapa Usuário → Objetivo do técnico
- Objetivo de longo prazo: facilitar o gerenciamento de chamados de serviço
- Foco do sprint (circulado no mapa): **visualizar os chamados pendentes**
- HMWs mais votadas: status em tempo real · técnico com todas as informações · otimizar rotas
- O sprint mirou um único alvo — decisão de método (não retrofitamos o supervisor)

## 6 · O protótipo
- Fluxo do técnico (mobile): login → chamados do dia → rota no mapa → encerrar/reagendar
- Supervisor (web): painel da operação que cria e distribui os chamados (a origem do fluxo)
- Telas de alta fidelidade no Figma
- O chamado criado pelo supervisor aparece na lista do técnico → fecha o loop

## 7 · Teste de usabilidade + UX: método *(2.2)*
- Participantes: 5, anônimos (P1–P5), com familiaridade digital variada
- Técnica de usabilidade: **Teste por tarefas com Think-Aloud** (pensar em voz alta)
- Técnica de UX: **UEQ-S** (questionário de experiência do usuário)
- Tarefas: T1 login · T2 ver chamados pendentes · T3 buscar chamado · T4 rota no mapa · T5 encerrar/reagendar
- *(detalhes em `fase4-teste-usabilidade-ux.md`)*

## 8 · Resultados: defeitos encontrados *(2.3)* — **[A PREENCHER após o teste]**
- 3 a 5 defeitos de usabilidade
- Cada defeito com a heurística de Nielsen violada
- Severidade de cada defeito (escala 0–4)
- Evidência: em qual tarefa os participantes travaram

## 9 · Melhorias e resultados de UX *(2.3)* — **[A PREENCHER]**
- Antes → Depois: screenshot do problema e a correção no protótipo
- Resultados do UEQ-S: médias de qualidade pragmática e hedônica
- Interpretação: positiva (> 0,8) · neutra · negativa

## 10 · Obrigado · Demonstração *(2.4)*
- Demonstração ao vivo: **landing page**, **vídeo** e **protótipo final**
- Landing page: https://pedroh-tardivo.github.io/track-fibra
- Protótipo (Figma): https://www.figma.com/design/WlkwUAUbbs0dsNf184dEUv
- Equipe de IHC — UTFPR Campo Mourão · 2026

---

### Lembretes para a apresentação
- ⏱ **Máximo 15 min** (−0,5 ponto por minuto excedente).
- Ao final: apresentar landing + vídeo + **demo do protótipo** (vale 50 pts).
- Critérios do protótipo: usabilidade pelas heurísticas de Nielsen + consistência com o Design Sprint.
