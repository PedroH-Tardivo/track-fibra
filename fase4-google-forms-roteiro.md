# Fase 4 — Montar o questionário no Google Forms (passo a passo)

> **Divisão recomendada (híbrido):**
> - **Google Forms** = o que o **participante** responde → perfil + UEQ-S + perguntas abertas.
> - **Google Sheets** = o que o **moderador** anota ao vivo (sucesso/erros/tempo por tarefa) + a análise. Use o arquivo [`fase4-coleta-dados.xlsx`](fase4-coleta-dados.xlsx) — ele **abre direto no Google Sheets** (Arquivo → Importar planilha, ou clicar com o botão direito → Abrir com → Google Sheets). As fórmulas (médias do UEQ-S, resumo por tarefa) funcionam igual.

---

## Configuração inicial do Form
1. Acesse **forms.google.com** → **Em branco**.
2. Engrenagem **⚙ (Configurações)**:
   - **Coletar endereços de e-mail: DESLIGADO** (o teste é **anônimo**).
   - **Limitar a 1 resposta: DESLIGADO** (senão exige login Google).
3. **Título:** `Track Fibra — Avaliação do Protótipo (UX)`
4. **Descrição:** *"Você está avaliando um aplicativo em protótipo. Não há resposta certa ou errada. Suas respostas são anônimas."*

---

## Seção 1 — Identificação e consentimento
- **Código do participante** · tipo *Resposta curta* · obrigatória → o moderador escreve `P1`…`P5`.
- **Consentimento** · tipo *Caixas de seleção* · 1 opção:
  - ☐ "Autorizo a gravação da tela/áudio da sessão e entendo que meus dados são anônimos."

## Seção 2 — Perfil do participante *(anônimo — sem nome)*
- **Faixa etária** · *Múltipla escolha*: `18–25` · `26–35` · `36–45` · `46+`
- **Escolaridade / área de atuação** · *Resposta curta*
- **Familiaridade digital (autoavaliação)** · *Múltipla escolha*: `Baixa` · `Média` · `Alta`
- **Já usa app/sistema no trabalho?** · *Múltipla escolha*: `Sim` · `Não` (ativar opção "Outro" p/ qual)
- **Como usa o celular no trabalho?** · *Múltipla escolha*: `Duas mãos` · `Uma mão` · `Apoiado`

## Seção 3 — UEQ-S (experiência) → use **Grade de múltipla escolha**
Tipo de pergunta: **Grade de múltipla escolha** · marque **"Exigir uma resposta por linha"**.

- **Colunas (7):** `-3` · `-2` · `-1` · `0` · `1` · `2` · `3`
- **Linhas (8)** — coloque o par nos extremos no próprio texto da linha:

| # | Linha (texto a digitar) | Dimensão |
|---|---|---|
| 1 | `atrapalha  →  apoia / dá suporte` | pragmática |
| 2 | `complicado  →  fácil` | pragmática |
| 3 | `ineficiente  →  eficiente` | pragmática |
| 4 | `confuso  →  claro` | pragmática |
| 5 | `maçante  →  empolgante` | hedônica |
| 6 | `desinteressante  →  interessante` | hedônica |
| 7 | `convencional  →  inventivo / criativo` | hedônica |
| 8 | `usual  →  inovador / de ponta` | hedônica |

> Mantenha **esta ordem** (1–4 pragmáticas, 5–8 hedônicas) para a análise bater com a planilha. `-3` é sempre o polo negativo (esquerda) e `+3` o positivo (direita).

## Seção 4 — Perguntas abertas
Tipo *Parágrafo* nas três:
1. O que foi **mais fácil** e o que foi **mais confuso**?
2. Faltou alguma **informação** em alguma tela?
3. Você **usaria isto no dia a dia**? Por quê?

---

## Como analisar depois
1. No Form: aba **Respostas → Vincular ao Planilhas** (cria a planilha de respostas).
2. Para o **UEQ-S**, adicione 3 colunas na planilha de respostas:
   - **Pragmática** = `MÉDIA(` colunas dos itens 1–4 `)`
   - **Hedônica** = `MÉDIA(` colunas dos itens 5–8 `)`
   - **Geral** = `MÉDIA(` todos os 8 `)`
   - *(as respostas da grade vêm como `-3…3`; se vierem como texto, troque por número antes da média)*
   - Alternativa: colar as respostas no **Excel oficial do UEQ-S** (ueq-online.org) para o benchmark.
3. As **métricas por tarefa** (sucesso/erros/tempo) ficam na aba `Coleta_Tarefas` do `fase4-coleta-dados.xlsx` (Google Sheets), preenchidas pelo moderador durante a sessão.
4. Os **3–5 defeitos** (antes/depois + heurística + severidade) vão na aba `Defeitos`.

> **Resumo:** Form para o participante · Sheets para o moderador e a análise. É o mesmo conteúdo dos arquivos [`fase4-formulario-ueq-s.html`](fase4-formulario-ueq-s.html) (versão imprimível, caso prefiram papel) e [`fase4-coleta-dados.xlsx`](fase4-coleta-dados.xlsx).
