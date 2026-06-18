# CLAUDE.md — Track Fibra (Trabalho Final de IHC)

Documento de referência para a execução do trabalho final da disciplina de **Interação Humano-Computador** (UTFPR – Campo Mourão, BCC, 2026). Reúne **todas as etapas, passos e requisitos** definidos nas instruções do professor, com a pontuação de cada item.

> **Contexto do produto:** **Track Fibra** — Sistema de Gerenciamento de Chamadas de Serviço para Provedores de Internet (web + mobile).
> **Equipe:** Kauan Silva Schiavon · Leonardo Hideki Gen Sato · Pedro Henrique Tardivo Rodrigues · Guilherme Fiuza R. P. de Carvalho.
> Material de apoio já transcrito em [`transcricao-design-sprint.md`](transcricao-design-sprint.md).

---

## 0. Regra de pontuação geral

- São **duas entregas**, cada uma valendo **100 pontos**.
- **Nota final = (Entrega 1 + Entrega 2) ÷ 2.**
- A apresentação tem **tempo máximo de 15 minutos**.
  - **Penalidade: −0,5 ponto a cada minuto excedente.**

| Entrega | Pontos | O que é |
|---|---|---|
| 1 | 100 | Landing page (GitHub Pages ou outra hospedagem) |
| 2 | 100 | Apresentação de slides + demonstração do protótipo |

---

## ENTREGA 1 — Landing Page (100 pontos)

Landing page hospedada no **GitHub Pages** (ou outro site de hospedagem).
Referências de exemplo: **AdaptWrite**, **Sphere**.

### 1.1 — Vídeo de conceito do produto (50 pontos)
- Vídeo **curto, no máximo 2 minutos**, **incorporado (embarcado) à página**.
- Estilo: vídeo de **demonstração do produto**, **chamativo e até cômico**.
- **Exceção para individual/dupla** (somente estes casos): pode ser algo mais simples, ex.: vídeo em formato de **slides** apresentando o produto. **Pode usar vídeos gerados por IA.**

**Checklist:**
- [ ] Vídeo com duração ≤ 2 min
- [ ] Embarcado na própria landing page
- [ ] Apresenta/demonstra o produto de forma chamativa

### 1.2 — Breve descrição do produto e diferenciais (10 pontos)
- [ ] Descrição curta do produto
- [ ] Diferenciais destacados

### 1.3 — Artefatos elaborados no Design Sprint (30 pontos)

**a) Mapeamento do problema (Mapa Usuário → Objetivo)** — deve conter:
- [ ] **Objetivo a longo prazo**
- [ ] **Cenários pessimistas**
- [ ] **HMWs escolhidas** (How Might We)
- [ ] **Foco do sprint circulado no mapa**

**b) Esboços das soluções votadas**
- [ ] Esboços (sketches) das soluções que foram votadas

**c) Storyboard**
- [ ] Storyboard da solução

> Fonte do conteúdo: seções 1–4 de [`transcricao-design-sprint.md`](transcricao-design-sprint.md).

### 1.4 — Integrantes da equipe (5 pontos)
- [ ] **Nome** de cada integrante
- [ ] **Foto** de cada integrante

### 1.5 — Protótipo do Figma (5 pontos)
- [ ] Protótipo do Figma **embarcado na página** **OU** link para o repositório no GitHub

### Resumo de pontos — Entrega 1
| Item | Pontos |
|---|---|
| Vídeo de conceito (≤2 min, embarcado) | 50 |
| Descrição do produto + diferenciais | 10 |
| Artefatos do Design Sprint (mapa + esboços + storyboard) | 30 |
| Integrantes (nome + foto) | 5 |
| Protótipo do Figma (embarcado ou link) | 5 |
| **Total** | **100** |

---

## ENTREGA 2 — Apresentação de Slides + Demonstração (100 pontos)

Slides com o conteúdo abaixo **+ demonstração do protótipo**.

### 2.1 — Visão geral da solução e motivação (10 pontos)
- [ ] Breve descrição da solução
- [ ] **Principais resultados do pré-sprint** (motivação)
- [ ] Problemas, oportunidades e/ou necessidades identificadas

> Fonte: seção 5 de [`transcricao-design-sprint.md`](transcricao-design-sprint.md).

### 2.2 — Teste de usabilidade + Avaliação de UX (10 pontos)
- [ ] **Perfil dos participantes** do teste — **sem identificação pessoal!**
- [ ] **Técnicas utilizadas:**
  - [ ] **1 técnica de teste de usabilidade**
  - [ ] **1 técnica de UX**
- [ ] **Lista de tarefas** realizadas pelo participante (para o teste de usabilidade)

### 2.3 — Resultados do teste + melhorias no protótipo (30 pontos)
- [ ] **Problemas identificados: 3 a 5 defeitos**
- [ ] Para cada problema: **screenshot do problema** seguido de **como foi corrigido** no protótipo (**antes e depois**)
- [ ] **Resultados da avaliação de UX**
- [ ] **Link para a landing page e para o protótipo** ao final dos slides

### 2.4 — Apresentação (50 pontos)
Ao final da apresentação, a equipe deve:
- [ ] Apresentar a **landing page** do projeto
- [ ] Apresentar o **vídeo**
- [ ] Fazer a **demonstração do protótipo final**

**Critérios de avaliação do protótipo:**
- **Usabilidade** à luz das **heurísticas de Nielsen**
- **Consistência** do protótipo com as decisões tomadas nas etapas do Design Sprint

**Tempo:**
- ⏱ **Máximo 15 minutos** — desconta **0,5 ponto por minuto excedente**.

### Resumo de pontos — Entrega 2
| Item | Pontos |
|---|---|
| Visão geral da solução + motivação (pré-sprint) | 10 |
| Teste de usabilidade + avaliação de UX (perfil, técnicas, tarefas) | 10 |
| Resultados do teste + melhorias (3–5 defeitos antes/depois) + UX + links | 30 |
| Apresentação (landing page + vídeo + demo do protótipo) | 50 |
| **Total** | **100** |

---

## Perfil Supervisor (web) — decisão e plano por fase

> **Decisão (jun/2026):** adicionar o perfil **supervisor** ao produto como **fluxo secundário em versão *web*** — **não** como segundo foco do Design Sprint. O foco do sprint **continua sendo o técnico** (etapa *visualizar chamados pendentes*). O supervisor entra como **a outra ponta do mesmo fluxo** (a origem dos chamados) e como a **versão web** já prevista no pré-sprint.

**Por que assim (consistência — critério avaliado na Entrega 2):**
- O mapa Usuário→Objetivo é **"Técnico → Objetivo"**; o **foco circulado** é só *visualizar chamados pendentes*; as **5 telas votadas** e o **storyboard** são todos do técnico (mobile). Retrofitar o sprint pra incluir o supervisor **criaria inconsistência**.
- O **pré-sprint já justifica** o supervisor ser **web** ("supervisores: 100% usam computador → confirma versão web") e já lista as dores dele (falta de visibilidade da operação). Logo, o supervisor é **escopo de produto**, não improviso.
- **Regra de ouro:** **não** mexer no círculo de foco nem na lista de "soluções votadas" do Miro. O supervisor é complemento; mostrar que o sprint focou em um alvo **ganha** ponto de método.

**Telas mínimas do supervisor (web, ~1440×900):**
1. **Login do Supervisor (web)** — card central, mesma marca (refazer o login supervisor que estava mobile).
2. **Painel da Operação (dashboard)** — barra lateral + tabela de chamados do dia (status Pendente/Em andamento/Concluído) + filtros + **mapa com técnicos** (a "visibilidade em tempo real" pedida pelos supervisores).
3. **Novo Chamado / Distribuir** — formulário (cliente, endereço, tipo, técnico, prioridade). Ao salvar, **o chamado entra na lista de pendentes do técnico** → fecha o loop com o foco do sprint.

**Narrativa da demo (loop):** Supervisor cria o chamado (web) → aparece em *chamados pendentes* do técnico (foco, mobile) → técnico executa e encerra → status volta ao painel do supervisor.

**Impacto por fase:**
| Fase | Impacto | Ação |
|---|---|---|
| 1 · Protótipo (Figma) | Médio | Criar as 3 telas **web** (frames desktop, **não** mobile), mesma identidade (Inter, #1D4ED8/#06B6D4). Ligar navegação interna. Atenção ao limite do MCP Figma (Starter) — fazer incremental. |
| 2 · Artefatos (Miro) | Mínimo | **Não** alterar foco nem "soluções votadas". No máximo, anotação leve: *"Supervisor (web) — origem dos chamados"* como ator a montante do mapa/storyboard. |
| 3 · Landing + Vídeo | Positivo | Subseção **"Para o supervisor (web)"** com mockup de navegador; reforça o "2 perfis · web + mobile" já prometido. Roteiro do vídeo ganha o gancho supervisor→técnico. |
| 4 · Teste + UX | Decisão de escopo | **Recomendado:** teste **principal = técnico**; **opcional** 2–3 tarefas curtas do supervisor (login web → criar chamado → acompanhar status). |
| 5 · Correções + Slides | Leve | Slide "Dois perfis, um produto" + slide explicando **por que o sprint focou no técnico** (método). Defeitos saem do fluxo testado. |

**Tempo:** a banca tem teto de 15 min → supervisor entra como **beat curto da demo** (1–2 telas), não como passeio completo.

### Status do supervisor (jun/2026)
- [x] **Landing** — seção `#supervisor` publicada (painel mockup HTML/CSS dentro de janela de navegador). No ar.
- [ ] **Figma — A FAZER DEPOIS** — criar as 3 telas web (Login Supervisor, Painel da Operação, Novo Chamado/Distribuir) em frames desktop e ligar a navegação. **Bloqueado pelo limite do MCP Figma (plano Starter)** — refazer quando a cota resetar ou após upgrade do plano.
- [ ] **Miro — A FAZER DEPOIS** — apenas a anotação leve *"Supervisor (web) — origem dos chamados"* como ator a montante. **Não** mexer no foco circulado nem na lista de "soluções votadas".

---

## Checklist mestre de pendências

**Entrega 1 — Landing page**
- [ ] Hospedagem definida (GitHub Pages ou outra) e no ar
- [ ] Vídeo conceito (≤2 min) produzido e embarcado
- [ ] Descrição + diferenciais escritos
- [ ] Mapa Usuário→Objetivo (objetivo LP, cenários pessimistas, HMWs, foco circulado)
- [ ] Esboços das soluções votadas
- [ ] Storyboard
- [ ] Nomes + fotos dos 4 integrantes
- [ ] Figma embarcado ou link do repositório

**Entrega 2 — Slides + apresentação**
- [ ] Visão geral + motivação (pré-sprint)
- [ ] Perfil dos participantes do teste (anônimo)
- [ ] 1 técnica de teste de usabilidade + 1 técnica de UX
- [ ] Lista de tarefas do teste
- [ ] 3 a 5 defeitos com antes/depois (screenshots)
- [ ] Resultados da avaliação de UX
- [ ] Links (landing page + protótipo) no final
- [ ] Ensaiar para ficar **dentro de 15 min**
- [ ] Demo do protótipo final pronta

> **Pendências que ainda dependem de execução do grupo (não derivam dos artefatos atuais):** realizar o teste de usabilidade e a avaliação de UX, definir as técnicas, registrar perfil dos participantes e tarefas, capturar screenshots antes/depois das correções, finalizar o protótipo no Figma e gravar o vídeo conceito.
