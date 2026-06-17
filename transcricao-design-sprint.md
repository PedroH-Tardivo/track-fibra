# Track Fibra — Transcrição dos Artefatos do Design Sprint

> Transcrição feita a partir das fotos dos artefatos físicos + Relatório de Pré-sprint.
> Trechos marcados com `(?)` estavam pouco legíveis na foto (lápis claro / ângulo) e podem precisar de conferência.

## Identificação do projeto
- **Produto:** **Track Fibra** — Sistema de Gerenciamento de Chamadas de Serviço para Provedores de Internet (plataformas **web + mobile**).
- **Instituição:** UTFPR – Campo Mourão · Bacharelado em Ciência da Computação · Interação Humano-Computador · 2026.
- **Equipe:**
  - Kauan Silva Schiavon
  - Leonardo Hideki Gen Sato
  - Pedro Henrique Tardivo Rodrigues
  - Guilherme Fiuza R. P. de Carvalho
- **Dois perfis de usuário:**
  - **Técnico de campo** (app mobile) — executa as chamadas em campo.
  - **Supervisor / despachante** (sistema web) — cria, distribui e acompanha as chamadas.
- **Três tipos de chamada:** instalação, manutenção e recolher equipamento.

---

## 1. Mapeamento do Problema (Mapa Usuário → Objetivo)

### Objetivo a longo prazo
> **Facilitar o gerenciamento de chamados de serviço para provedores de internet** *(prestadores de serviço)*.

### Mapa / fluxo do usuário (Técnico → Objetivo)
Fluxo principal mapeado:

```
TÉCNICO
   │
   ▼
FAZ O LOGIN
   │
   ▼
VISUALIZA OS CHAMADOS PENDENTES
   │
   ▼
CONFIRMA A SUGESTÃO DA ROTA DO DIA
   │
   ▼
FAZ UMA VISITA AO LOCAL E VERIFICA
SE É POSSÍVEL REALIZAR O SERVIÇO
   │
   ├──► REALIZA O SERVIÇO ──► ENCERRA O CHAMADO   ✅ (caminho feliz)
   │
   └──► NÃO REALIZA NO MOMENTO ──► FAZ O REAGENDAMENTO  ↺ (volta ao fluxo)
```

### Foco do sprint
O foco circulado no mapa concentra-se na etapa de **visualizar os chamados pendentes** — o momento em que o técnico precisa ter, de forma clara e confiável, todas as informações do dia (ataca direto as dores do pré-sprint: falta de informação organizada e dependência da memória/WhatsApp).
---

## 2. Perguntas do Sprint / Cenários Pessimistas

### HMWs escolhidas (com votação por pontos)
Post-its priorizados (número de votos = pontos colados):

| Pergunta (Como Poderíamos / HMW) | Votos | Observação |
|---|---|---|
| Como poderíamos **verificar o status do chamado em tempo real**? | ●●●● (4) | mais votada |
| Os **técnicos terão todas as informações** para realizar um serviço? | ●●●● (4) | |
| Como poderíamos **otimizar as rotas**? | ●●●● (4) | |
| **Empresas de grande porte dominarão o setor?** | ●● (2) | *"Eles já costumam ter software próprio"* |
| Os **funcionários estarão dispostos a mudar o procedimento atual?** | ●● (2) | *"Planilhas e WhatsApp"* (procedimento atual) |
| Como poderíamos **garantir que as alterações cheguem ao técnico**? | ●● (2) | |
| Como poderíamos **atender técnicos com pouca familiaridade digital**? | ● (1) | |


### Demais perguntas / cenários pessimistas levantados (mural amarelo)
- Os técnicos gostam da ideia de serem "fiscalizados"o tempo todo? `(?)`
- Terá suporte para enviar diversos chamados simultaneamente?
- Se a demanda aumentar, conseguirá acompanhar?
- Os usuários conseguirão aprender e utilizar o aplicativo com facilidade?
- Conseguiriamos acompanhar as mudanças de mercado? `(?)`
- Cada cliente exigirá atenção/personalização — muito por ser personalizado? `(?)`
- Como vamos passar confiança para contratarem nosso sistema?
- O cliente vai preferir pessoas/empresas mais experientes para construir o aplicativo? `(?)`

---

## 3. Esboços das Soluções Votadas (Wireframes)

5 telas esboçadas em papel (lápis). Telas reconstruídas:

### Tela 1 — LOGIN
- Título: **LOGIN**
- Campo: **Nome de usuário**
- Campo: **Senha** — link *"Esqueci a senha"* ao lado `(?)`
- ☐ **Continuar conectado**
- Botão: **Entrar**

### Tela 2 — Lista de Chamados / Buscar
- Barra de busca: 🔍 **Buscar...**
- **≡ Filtrar**
- Lista de cards de chamados (cada um com menu suspenso `▾`):
  - **1º Chamado** — Cliente: __ · Endereço: __ · Tipo: __ · ◯ **Pendente**
  - **2º Chamado** — Cliente: __ · Endereço: __ · Tipo: __ · ◯ **Pendente**
  - **3º Chamado** — Cliente: __ · Endereço: __ · Tipo: __ · ◯ **Pendente**
  ...

### Tela 3 — Mapa / Rota do dia
- **Mapa** com marcadores de localização (pins) dos chamados
- **1º Chamado** · **Em andamento** ⊙
- Cliente: **Jorge da Silva Bueno** — Tipo: **Manutenção**
- (outro chamado) **Júlio de Oliveira Carneiro, 299 — Novo Yorque** `(?)`
- Botão: **Adicionar Observação** `(?)`  · botão **Alterar Rota** `(?)`

### Tela 4 — Detalhe / Encerrar Chamado
- Título: **ENCERRAR CHAMADO #183AC3** `(?)`
- 📍 **Endereço:** Av. Paraná, 199
- 🔧 **Tipo:** Instalação
- 👤 **Cliente:** Jorge
- 📝 **OBS:** *"Trazer 10m de cabo... segurança... com defeito"* `(?)`
- ⏱ **Hora início: 10:00**
- Botões: **REAGENDAR** | **FINALIZAR**

---

## 4. Storyboard

O storyboard segue diretamente o fluxo do mapa, encadeando as 5 telas:

1. **Login** — o técnico abre o app e faz login (Tela 1).
2. **Chamados pendentes** — visualiza a lista de chamados do dia (Tela 2).
3. **Rota do dia** — confirma a sugestão de rota no mapa (Tela 3).
4. **Atendimento** — vai ao local e abre o detalhe do chamado (Tela 4).
5. **Decisão:**
   - **Realiza o serviço → Finaliza/Encerra o chamado**, ou
   - **Não realiza agora → Reagenda** (volta para a lista).

---

## 5. Síntese do Pré-sprint (motivação / resultados da coleta)

> Fonte: *Relatório de Pré-sprint – Síntese dos resultados*. Serve de **motivação** para o sprint.

### Método da coleta
- **Técnica:** 2 questionários estruturados (Google Forms), 1 por perfil, **14 questões cada** (escolha única/múltipla, faixa de valores, escala Likert e abertas).
- **Amostra:** **17 respondentes** → **12 técnicos de campo** + **5 supervisores/despachantes**.
- **Distribuição:** WhatsApp/contatos profissionais (via proprietário do provedor **NetFibra**); coleta de ~1 semana; respostas anônimas.
- **Análise:** quantitativa (frequência das alternativas, gráficos do Forms) + qualitativa (agrupamento das abertas por tema), **sem uso de IA**. Códigos T1–T12 (técnicos) e S1–S5 (supervisores).

### Perfil dos participantes
- **Técnicos:** maioria com até 30 anos; experiência equilibrada (metade até 3 anos, metade 4+); **instalação** é o tipo mais atendido (9/12); recebem chamadas **concentradas no WhatsApp**, sem sistema dedicado; familiaridade digital heterogênea (dificuldade concentrada em >30 anos); usam o celular variando entre apoiado e **uma só mão** → pede botões grandes e fluxo simples.
- **Supervisores:** coordenam de 3 a 10 técnicos; fluxo uniforme = central repassa → registra em **planilha** → distribui por **WhatsApp** (4/5 usam planilha+WhatsApp, nenhum usa software dedicado); monitoramento intenso (todos contatam técnicos várias vezes/dia); **100% usam computador** → confirma versão web.

### Principais resultados (dores)
- **Falta de fonte única e confiável de informação:** todos os 12 técnicos já se deslocaram em vão por dados incorretos/incompletos.
- **Falta de visibilidade da operação:** supervisor não sabe onde o técnico está nem o status → cobrança manual constante pelo WhatsApp.
- **Dependência da memória + ausência de organização de rota:** item **pior avaliado** pelos técnicos na Likert.
- **Comunicação lenta e retrabalho:** respostas demoradas, mudanças de última hora não chegam de forma confiável, deslocamentos desnecessários.

### Funcionalidades mais valorizadas
- **Técnicos:** ver a lista do dia, notificações em tempo real, registrar fotos/observações, navegação por mapa/GPS — e, em destaque nas abertas, **rota automática otimizada**.
- **Supervisores:** acompanhar o **status** de cada chamada e ver a **localização dos veículos no mapa** (localização em tempo real quase unânime).

### Citações representativas
- T1 — *"Lembrar a ordem das chamadas e o endereços delas."* (dependência da memória)
- T6 — *"Informações incompletas sobre o cliente, localização errada e mudanças de rota durante o dia."* / *"Aplicativo lento ou travando durante deslocamento."* / *"Rota automática otimizada entre atendimentos."*
- T7 — *"Interface complicada com muitas telas e excesso de informações."*
- S1 — *"Preciso cobrar os técnicos pelo WhatsApp o tempo todo para saber se eles já chegaram no cliente..."* / *"Se for pro sistema não mostrar as informações certas, é melhor continuar do jeito que está."*
- S3 — *"Os técnicos não avisam sobre o andamento do serviço."*
- S5 — *"Conseguir visualizar em tempo real a localização e qual a chamada que o técnico está operando."*

### Conclusão (motivação do sprint)
Problema **real e compartilhado** pelos dois perfis. Para o **técnico**, o Track Fibra deve ser um **organizador confiável do dia de trabalho**; para o **supervisor**, uma **central de visibilidade da operação**. Há boa receptividade: ambos concordam que uma ferramenta dedicada tornaria o trabalho mais eficiente.

---

### Inventário das fotos
| Foto | Conteúdo |
|---|---|
| (mural verde/laranja) | HMWs escolhidas com votação por pontos |
| IMG_9904 | Objetivo a longo prazo + mural de perguntas/cenários |
| IMG_9906 | Mapa Usuário → Objetivo (fluxo) |
| IMG_9901 | Esboço — Tela LOGIN |
| IMG_9903 | Esboço — Lista de Chamados / Buscar |
| IMG_9902 | Esboço — Mapa / Rota |
| IMG_9900 | Esboço — Detalhe / Encerrar Chamado |
| IMG_9899 | Folha-resumo com as 4 telas juntas |
