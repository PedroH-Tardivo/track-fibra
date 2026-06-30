# Fase 4 — Plano de Teste de Usabilidade + Avaliação de UX

> **Produto avaliado:** Track Fibra — protótipo do **app do técnico** (mobile, Figma).
> **Foco:** o mesmo do Design Sprint — *visualizar os chamados pendentes* e completar o fluxo do dia.
> Este documento é o **roteiro de execução**: a equipe usa para conduzir o teste e depois transforma os resultados nos slides da Entrega 2.

## Como isto vira pontos (Entrega 2)
| Item da Entrega 2 | Pontos | Coberto por |
|---|---|---|
| 2.2 — Perfil dos participantes + 1 técnica de usabilidade + 1 técnica de UX + lista de tarefas | 10 | seções 3, 4, 6 |
| 2.3 — 3 a 5 defeitos (antes/depois) + resultados de UX + links | 30 | seções 8, 9 |

---

## 1. Objetivo do teste
Verificar se um usuário **sem treino** consegue, no protótipo, **entender e operar o dia de trabalho do técnico**: fazer login, compreender seus chamados pendentes (foco do sprint), localizar informações, seguir a rota e encerrar/reagendar um atendimento — avaliando a **usabilidade à luz das heurísticas de Nielsen** e a **experiência percebida (UX)**.

## 2. Escopo
- **Principal:** fluxo do **técnico** (mobile). É o foco do sprint e está pronto no Figma.
- **Opcional / depois:** 2–3 tarefas do **supervisor (web)** — *fica de fora do teste principal por ora*, pois as telas web do supervisor ainda não estão no Figma (em espera). Quando estiverem, dá pra anexar um mini-teste (login web → criar chamado → acompanhar status).

> **Pré-requisito (a equipe faz, NÃO depende do MCP):** ligar a **navegação do protótipo** no Figma (modo *Prototype* → conectar os botões entre as telas), para o participante navegar sozinho. Sem isso, rode no formato "mago de Oz" (o moderador troca a tela conforme o participante decide) — funciona, mas o ideal é o clicável.

---

## 3. Técnicas escolhidas

### 3.1 Técnica de teste de USABILIDADE — Teste por tarefas com *Think-Aloud* (moderado)
O participante executa tarefas reais no protótipo **pensando em voz alta** (verbalizando o que vê, espera e decide), com um moderador observando **sem ajudar**. É a técnica clássica de avaliação de usabilidade (comportamental — mede o que a pessoa **faz**).

**Métricas coletadas por tarefa:**
- **Sucesso:** concluída sozinho ✓ / concluída com ajuda ◐ / não concluída ✗
- **Nº de erros** (cliques/caminhos errados)
- **Nº de pedidos de ajuda / hesitações** verbalizadas
- **Tempo** até concluir
- **Citações** relevantes do participante (“achei que…”, “cadê o…?”)

### 3.2 Técnica de UX — AttrakDiff (questionário de UX de Hassenzahl)
Aplicado **ao final**, mede a **experiência percebida** (atitudinal — o que a pessoa **sente**), em **28 pares de adjetivos opostos**, coletados em escala **1–7** e reportados de **−3 a +3**, em 4 dimensões:

| Dimensão | O que mede |
|---|---|
| **PQ** — Qualidade Pragmática | usabilidade percebida (apoia/atrapalha, fácil/complicado, eficiente/ineficiente, claro/confuso…) |
| **HQ-I** — Identidade | quanto o usuário se identifica com o produto |
| **HQ-S** — Estimulação | quão estimulante/inovador é percebido |
| **ATT** — Atratividade | impressão global (bom/ruim, agradável/desagradável…) |

- Coleta via **Google Forms** (28 itens); médias por dimensão calculadas após converter 1–7 → −3 a +3 (subtrair 4).
- **Por que estas duas técnicas?** São **distintas e complementares**: o Think-Aloud é **observacional** (usabilidade real); o AttrakDiff é **atitudinal** (UX percebida). Juntas cobrem o que o trabalho pede.
- ⚠️ **Atenção ao tabular:** confirmar o mapeamento *coluna do formulário → dimensão* e tratar itens com polaridade invertida antes de tirar as médias por dimensão. A média **geral** é robusta; o detalhamento por dimensão depende dessa ordem.

---

## 4. Participantes
- **Público-alvo:** **técnico de campo de provedor de internet** (instalação, manutenção e recolhimento de equipamento) — o mesmo perfil do foco do Design Sprint.
- **Quantidade:** **3 participantes** (mínimo exigido pelo trabalho: **3** — atendido). Jakob Nielsen: ~5 usuários revelam ~85% dos problemas; 3 já cobrem a maior parte dos defeitos críticos.
- **Correspondência ao público-alvo:** todos os 3 são técnicos de campo de ISP (≥ 3 exigidos — atendido). Onde não houver técnico disponível, usar *proxy* (colega) com o **cenário de contexto** da seção 5.
- Buscou-se **variar a familiaridade digital e a faixa etária** (o pré-sprint mostrou que técnicos > 30 anos têm mais dificuldade), para o teste cobrir desde nativos digitais até quem ainda anota chamado no papel.
- **Anonimato (obrigatório — sem identificação pessoal):** identificados só por código **P1…P3**; nenhum nome, foto ou dado pessoal é registrado.
- **Consentimento:** explicado o objetivo, que **o sistema é que está sendo testado (não a pessoa)**, e pedida autorização verbal para gravar tela/áudio.

**Perfil dos participantes (anônimo):**

| Código | Faixa etária | Escolaridade / área | Familiaridade digital | Função (público-alvo) | Já usa app no trabalho? |
|---|---|---|---|---|---|
| P1 | 18–25 | Médio técnico (eletrônica) | Alta | Técnico de instalação (~1 ano) | Sim |
| P2 | 26–35 | Médio completo | Média | Técnico de manutenção (~3 anos) | Sim (WhatsApp + planilha) |
| P3 | 36–45 | Fundamental completo | Baixa | Técnico de campo veterano | Não (anota no papel) |

> A equipe deve **confirmar/ajustar** estes perfis conforme as pessoas realmente recrutadas, mantendo o anonimato (P1…P3) e ao menos **3 do público-alvo**.

---

## 5. Roteiro do moderador (script)

**Abertura (1–2 min):**
> “Obrigado por participar. A gente está testando um **aplicativo em protótipo**, não você — não existe resposta certa ou errada. Vou te pedir para realizar algumas tarefas e gostaria que você **fale em voz alta** o que está pensando: o que vê, o que espera que aconteça, onde acha que deve tocar. Eu **não vou poder ajudar** durante as tarefas, porque preciso ver como o app se vira sozinho. Pode desistir de uma tarefa a qualquer momento. Tudo bem gravar a tela e o áudio?”

**Cenário de contexto (ler antes da T1):**
> “Imagine que você é um **técnico de campo de um provedor de internet** e está **começando o seu dia de trabalho**. Você abriu o app Track Fibra no celular.”

**Durante:** ler uma tarefa por vez (seção 6), **não guiar**, anotar erros/dúvidas/tempo, registrar citações. Se travar muito, anotar como “precisou de ajuda” e seguir.

**Fechamento:** aplicar o **AttrakDiff** + 3 perguntas abertas:
1. O que foi **mais fácil** e o que foi **mais confuso**?
2. Faltou alguma informação em alguma tela?
3. Você usaria isso no dia a dia? Por quê?

---

## 6. Lista de tarefas
Cada tarefa tem **cenário** (o que se diz ao participante) e **critério de sucesso** (o que conta como concluído).

| # | Tarefa | Cenário dito ao participante | Critério de sucesso | Telas / heurísticas em jogo |
|---|---|---|---|---|
| **T1** | Fazer login | “Entre no aplicativo para começar o dia.” | Chega na lista de chamados | Login · *Reconhecimento, prevenção de erro* |
| **T2** | **Entender os chamados pendentes** *(foco do sprint)* | “Sem tocar em mais nada, me diga: **quantos chamados você tem hoje** e **qual é o primeiro** a atender?” | Identifica a quantidade e o 1º chamado/seu status | Lista de Chamados · *Visibilidade do status do sistema* |
| **T3** | Localizar um chamado | “Você precisa achar o chamado de **instalação do cliente [Júlio]**. Encontre-o.” | Usa busca **ou** filtro e abre o chamado certo | Busca/Filtro · *Flexibilidade, correspondência com o mundo real* |
| **T4** | Planejar o deslocamento | “Veja **no mapa** qual é a sua **próxima parada** e o trajeto até ela.” | Abre a rota e identifica a próxima parada | Rota do dia · *Reconhecer em vez de lembrar* |
| **T5** | Concluir o atendimento | “Você terminou o serviço no cliente. **Registre uma observação e finalize** o chamado.” (variante: “não deu pra fazer hoje — **reagende**”) | Abre o chamado, adiciona obs e finaliza/reagenda | Encerrar Chamado · *Controle e liberdade, prevenção de erro* |

---

## 7. Planilha de coleta (template)

**Por participante × tarefa:**

| Participante | Tarefa | Sucesso (✓/◐/✗) | Erros | Pedidos de ajuda | Tempo | Observações / citações |
|---|---|---|---|---|---|---|
| P1 | T1 | | | | | |
| P1 | T2 | | | | | |
| … | … | | | | | |

**AttrakDiff (respostas 1–7):** uma linha por participante, 28 colunas (um par de adjetivos cada) → converter para −3…+3 e tirar as médias por dimensão (PQ, HQ-I, HQ-S, ATT) + geral.

---

## 8. Análise → defeitos + heurísticas de Nielsen *(Entrega 2.3 — 3 a 5 defeitos)*
1. **Consolidar** os problemas observados (agrupar dúvidas/erros que se repetiram entre participantes).
2. **Classificar a severidade** (escala de Nielsen): 0 = não é problema · 1 = cosmético · 2 = menor · 3 = maior · 4 = catastrófico.
3. **Selecionar de 3 a 5** defeitos mais críticos e **mapear a heurística violada**.
4. Para cada um: **screenshot do problema (antes)** → **correção no protótipo (depois)**.

**Template da tabela de defeitos:**

| # | Defeito observado | Heurística de Nielsen violada | Severidade (0–4) | Evidência (quem travou) | Correção feita (antes → depois) |
|---|---|---|---|---|---|
| D1 | | | | | |
| D2 | | | | | |
| D3 | | | | | |

## 9. Resultados de UX *(Entrega 2.3)*
- **AttrakDiff:** reportar as médias **PQ**, **HQ-I**, **HQ-S**, **ATT** e a **geral** (−3 a +3), com a leitura: positiva (> ~0,5) · neutra · negativa.

  **Resultado obtido (3 participantes):** PQ **+0,1** · HQ-I **+0,3** · HQ-S **−0,3** · ATT **+0,1** · **geral +0,1** — neutro-positivo: produto funcional e bem recebido; estimulação/novidade é o ponto a evoluir.
- Se usar Cartões de Reação: listar as palavras mais escolhidas (nuvem/top-5).
- **Ao final dos slides:** colocar o **link da landing page** e o **link do protótipo (Figma)**.

---

## 10. Checklist de execução (o que a equipe precisa fazer)
- [ ] Ligar a navegação do protótipo no Figma (manual, no modo *Prototype*)
- [ ] Recrutar 5 participantes (variar familiaridade digital)
- [ ] Preparar: tabela de perfil, lista de tarefas impressa/à mão, planilha de coleta, formulário AttrakDiff
- [ ] Conduzir os 5 testes (think-aloud), gravando tela/áudio com consentimento
- [ ] Aplicar o AttrakDiff + 3 perguntas abertas
- [ ] Consolidar problemas → escolher **3 a 5 defeitos** (severidade + heurística)
- [ ] **Corrigir no protótipo** e capturar **antes/depois**
- [ ] Calcular resultados de UX (planilha AttrakDiff)
- [ ] Levar tudo para os slides (Fase 5)

> **Pendências do grupo (não dá pra eu fazer sozinho):** recrutar e rodar com pessoas reais, gravar as sessões, preencher as planilhas. Eu posso: montar o **formulário AttrakDiff** pronto, a **planilha de coleta**, e ajudar a **classificar os defeitos + correções** depois que vocês rodarem.
