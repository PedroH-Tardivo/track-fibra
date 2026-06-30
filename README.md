# Track Fibra

Sistema de Gerenciamento de Chamadas de Serviço para Provedores de Internet — trabalho final de **Interação Humano-Computador** (UTFPR – Campo Mourão, BCC, 2026).

**Landing page:** https://pedroh-tardivo.github.io/track-fibra/
**Protótipo (Figma):** https://www.figma.com/proto/WlkwUAUbbs0dsNf184dEUv/Track-Fibra?node-id=6-2&starting-point-node-id=6-2&scaling=scale-down-width

---

## O produto

Track Fibra é um app mobile para **técnicos de campo de provedores de internet**. Reúne num só lugar a lista de chamados do dia, a rota no mapa e o detalhe de cada atendimento — do login à conclusão do chamado.

**Fluxo principal:** Login → Lista de Chamados → Rota no Mapa → Detalhe → Finalizar / Reagendar

---

## Equipe

| Nome | Curso |
|---|---|
| Kauan Silva Schiavon | Ciência da Computação |
| Leonardo Hideki Gen Sato | Ciência da Computação |
| Pedro Henrique Tardivo Rodrigues | Ciência da Computação |
| Guilherme Fiuza R. P. de Carvalho | Ciência da Computação |

---

## Estrutura do repositório

```
index.html          — landing page (Entrega 1)
styles.css          — estilos da landing
assets/
  foto-*.jpg        — fotos da equipe
  proto-*.png       — prints do protótipo (Figma)
CLAUDE.md           — referência completa das entregas e requisitos
entrega2-slides-roteiro.md   — roteiro dos slides da Entrega 2
fase4-teste-usabilidade-ux.md — plano e resultados do teste de usabilidade
transcricao-design-sprint.md  — artefatos do Design Sprint (mapa, esboços, storyboard)
```

---

## Entregas

### Entrega 1 — Landing page (100 pts) ✅

| Item | Status |
|---|---|
| Vídeo de conceito (≤2 min, embarcado) | ✅ YouTube embed |
| Descrição do produto + diferenciais | ✅ |
| Artefatos do Design Sprint (mapa + esboços + storyboard) | ✅ via Miro embed |
| Integrantes (nome + foto) | ✅ |
| Protótipo do Figma embarcado | ✅ |

### Entrega 2 — Slides + apresentação (100 pts)

| Item | Status |
|---|---|
| Visão geral da solução + motivação (pré-sprint) | ✅ slides 2–5 |
| Perfil dos participantes (3 participantes, anônimos P1–P3) | ✅ slide 7 |
| Técnicas: Think-Aloud (usabilidade) + AttrakDiff (UX) | ✅ slide 7 |
| Lista de 5 tarefas do teste | ✅ slide 7 |
| 3 defeitos com antes/depois + resultados AttrakDiff | ✅ slides 8–9 |
| Links (landing page + protótipo) | ✅ slide 10 |
| Demo do protótipo ao vivo | a apresentar |

---

## Resultados do teste de usabilidade

**3 defeitos encontrados — todos corrigidos no protótipo:**

| # | Defeito | Heurística Nielsen | Severidade | Correção |
|---|---|---|---|---|
| D1 | Sem confirmação ao finalizar chamado | H5 — Prevenção de erros | 3 (major) | Botão "Desfazer" na tela de finalização |
| D2 | Números de telefone sem ação clicável | H4 — Consistência e padrões | 2 (minor) | Ícone de ligação clicável → tela "Ligando…" |
| D3 | Sem opção de adicionar fotos | H7 — Flexibilidade e eficiência | 2 (minor) | Botão "Adicionar foto" no detalhe do chamado |

**AttrakDiff (3 participantes, escala −3 a +3):**

| Dimensão | Média |
|---|---|
| PQ — Qualidade Pragmática | +0,1 |
| HQ-S — Estimulação | −0,3 |
| HQ-I — Identidade | +0,3 |
| ATT — Atratividade | +0,1 |
| **Geral** | **+0,1** |

Resultado neutro-positivo: app funcional e bem recebido pelo público-alvo; estimulação/novidade é a dimensão a melhorar em versões futuras.

---

## Rodar localmente

```bash
python3 -m http.server 8000
# abra http://localhost:8000
```
