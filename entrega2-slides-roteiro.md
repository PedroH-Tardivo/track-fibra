# Entrega 2 — Roteiro dos Slides (Track Fibra)

> Conteúdo aprovado dos 10 slides da apresentação (≤15 min). Estilo visual: **Sinal & Fibra** — navy `#0B1220`, azul `#1D4ED8`, ciano `#06B6D4`, geométrico com motivo de sinal.
> **Status:** a geração no Canva (IA) estava falhando no servidor (jun/2026) — roteiro guardado para regerar quando voltar, ou montar manualmente / via .pptx.
> Cobertura: itens 2.1 a 2.4 da Entrega 2. Slides 8 e 9 já preenchidos com os resultados reais (3 participantes, 3 defeitos com antes/depois, AttrakDiff).

---

## 1 · Track Fibra (capa)
- Sistema de gerenciamento de chamadas de serviço para provedores de internet — app mobile do técnico de campo
- Equipe: Kauan Silva Schiavon · Leonardo Hideki Gen Sato · Pedro Henrique Tardivo Rodrigues · Guilherme Fiuza R. P. de Carvalho
- UTFPR – Campo Mourão · Bacharelado em Ciência da Computação
- Interação Humano-Computador · 2026

## 2 · O problema *(2.1 — motivação)*
- O trabalho de campo é coordenado por planilha e WhatsApp, sem fonte única de informação
- Técnicos se deslocam à toa por dados incorretos ou incompletos
- Status e conclusões dependem de mensagens soltas, sem registro confiável
- Dependência da memória e ausência de rota organizada

## 3 · Pré-sprint: o que motivou *(2.1)*
- 2 questionários (Google Forms), 17 respondentes: 12 técnicos + 5 supervisores (via provedor NetFibra)
- Falta de fonte única e confiável de informação
- Falta de visibilidade do andamento dos atendimentos
- Dependência da memória e ausência de rota foi o item pior avaliado
- Técnicos trabalham o dia todo na rua → a solução é mobile, no celular

## 4 · A solução: Track Fibra *(2.1)*
- Um organizador confiável do dia de trabalho do técnico (app mobile)
- Tudo num só lugar: lista do dia, rota no mapa e detalhe de cada atendimento
- Do login à conclusão do chamado, com finalizar ou reagendar em um toque
- Três tipos de chamada: instalação, manutenção e recolhimento

## 5 · Design Sprint: foco no técnico *(consistência de método)*
- Mapa Usuário → Objetivo do técnico
- Objetivo de longo prazo: facilitar o gerenciamento de chamados de serviço
- Foco do sprint (circulado no mapa): **visualizar os chamados pendentes**
- HMWs mais votadas: status em tempo real · técnico com todas as informações · otimizar rotas
- O sprint mirou um único alvo, o técnico em campo — foco e consistência de método

## 6 · O protótipo
- Fluxo do técnico (mobile): login → chamados do dia → rota no mapa → detalhe → encerrar/reagendar
- 4 telas de alta fidelidade no Figma, com a identidade Sinal & Fibra
- Protótipo **100% navegável**: todo botão é clicável, como um app de verdade
- Demonstra o foco do sprint de ponta a ponta — do login à conclusão do chamado

## 7 · Teste de usabilidade + UX: método *(2.2)*

**Participantes — 3, anônimos (P1–P3), todos do público-alvo (técnico de campo de ISP):**

| | Faixa | Familiaridade digital | Função | Usa app no trabalho? |
|---|---|---|---|---|
| P1 | 18–25 | Alta | Técnico de instalação | Sim |
| P2 | 26–35 | Média | Técnico de manutenção | Sim |
| P3 | 36–45 | Baixa | Técnico veterano | Não (papel) |

*Sem identificação pessoal (só P1–P3). Mínimo exigido = 3; variamos faixa etária e familiaridade digital.*

**Técnicas (1 de usabilidade + 1 de UX):**
- **Usabilidade — Teste por tarefas com Think-Aloud** (moderado): o participante executa tarefas reais pensando em voz alta; o moderador observa sem ajudar. Mede o que a pessoa **faz** (sucesso, erros, hesitações, tempo).
- **UX — AttrakDiff** (questionário de UX de Hassenzahl): ao final, 28 pares de adjetivos opostos, coletados em escala 1–7 e reportados de −3 a +3, cobrindo 4 dimensões — PQ (qualidade pragmática), HQ-I (identidade), HQ-S (estimulação) e ATT (atratividade geral). Mede o que a pessoa **sente**.

**Lista de tarefas do teste:**
- **T1 — Login:** entrar no app para começar o dia → chega na lista de chamados
- **T2 — Chamados pendentes** *(foco do sprint)*: dizer quantos chamados há hoje e qual o primeiro a atender
- **T3 — Localizar chamado:** achar o chamado de instalação do cliente (Júlio) por busca ou filtro
- **T4 — Rota:** ver no mapa a próxima parada e o trajeto até ela
- **T5 — Concluir atendimento:** registrar observação e finalizar (ou reagendar) o chamado

*(roteiro do moderador, métricas e planilha de coleta em `fase4-teste-usabilidade-ux.md`)*

## 8 · Resultados: defeitos encontrados *(2.3)*

| # | Defeito observado | Heurística Nielsen | Severidade | Evidência | Correção |
|---|---|---|---|---|---|
| D1 | Sem confirmação ao finalizar chamado — participantes clicaram "Finalizar" sem perceber que a ação era irreversível | H5 — Prevenção de erros | **3** (major) | T5: todos os 3 Ps hesitaram ou expressaram dúvida ao finalizar | Tela "Chamado Finalizado" com botão **"Desfazer"** para reverter |
| D2 | Números de telefone sem ação clicável — participantes tentaram tocar no número esperando discar | H4 — Consistência e padrões | **2** (minor) | T3/T5: P1 e P2 tocaram no número sem resposta | Ícone de ligação clicável antes de cada número → tela "Ligando…" |
| D3 | Sem opção de adicionar fotos do atendimento — técnico não conseguia registrar evidência visual | H7 — Flexibilidade e eficiência | **2** (minor) | T5: P2 e P3 perguntaram "como mando uma foto?" | Botão **"Adicionar foto"** na tela de detalhe do chamado |

*Todos os 3 defeitos já corrigidos no protótipo final.*

## 9 · Melhorias e resultados de UX *(2.3)*

**Antes → Depois (screenshots em `assets/`):**

| Defeito | Antes | Depois |
|---|---|---|
| D1 — sem confirmação ao finalizar | `antes-d1-finalizado-sem-desfazer.png` (tela "Chamado finalizado!" sem opção de reverter) | `depois-d1-finalizado-com-desfazer.png` (mesma tela com link "Desfazer" acima do botão) |
| D2 — telefone sem ação | `antes-d2d3-detalhe-sem-icone-sem-foto.png` (campo Telefone como texto puro) | `depois-d2-detalhe-com-icone-ligar.png` (ícone azul clicável) + `depois-d2-ligando.png` (tela "Ligando…") |
| D3 — sem adicionar foto | `antes-d2d3-detalhe-sem-icone-sem-foto.png` (sem campo de mídia) | `antes-d2-depois-d3-detalhe-com-foto.png` (área "Adicionar foto do atendimento") |

**Resultados do AttrakDiff (3 participantes, escala -3 a +3):**

| Dimensão | Média | Interpretação |
|---|---|---|
| PQ — Qualidade Pragmática | **+0,1** | Levemente positiva — app funciona, tarefa é realizável |
| HQ-S — Estimulação | **−0,3** | Levemente negativa — percebido como convencional *(esperado para app utilitário v1)* |
| HQ-I — Identidade | **+0,3** | Positiva — técnicos se identificam com a proposta |
| ATT — Atratividade geral | **+0,1** | Levemente positiva — impressão global favorável |
| **Geral** | **+0,1** | Neutro-positivo — produto funcional e bem recebido pelo público-alvo |

*Interpretação: o produto cumpre sua proposta central (PQ e ATT positivos, HQ-I positivo). O HQ-S levemente negativo indica oportunidade de diferenciação visual/funcional em versões futuras — comum em primeiros protótipos de ferramentas utilitárias de campo.*

## 10 · Obrigado · Demonstração *(2.4)*
- Demonstração ao vivo: **landing page**, **vídeo** e **protótipo final**
- Landing page: https://pedroh-tardivo.github.io/track-fibra
- Protótipo (Figma): https://www.figma.com/proto/WlkwUAUbbs0dsNf184dEUv/Track-Fibra?node-id=6-2&starting-point-node-id=6-2&scaling=scale-down-width
- Equipe de IHC — UTFPR Campo Mourão · 2026

---

### Lembretes para a apresentação
- ⏱ **Máximo 15 min** (−0,5 ponto por minuto excedente).
- Ao final: apresentar landing + vídeo + **demo do protótipo** (vale 50 pts).
- Critérios do protótipo: usabilidade pelas heurísticas de Nielsen + consistência com o Design Sprint.
