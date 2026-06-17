# Track Fibra — Landing Page (Entrega 1)

Landing page do trabalho final de IHC (UTFPR – Campo Mourão).
Feita em HTML/CSS estático — pronta para **GitHub Pages**.

## Arquivos
- `index.html` — a página
- `styles.css` — estilos
- `assets/` — prints do protótipo (`proto-*.png`) e esboços do sprint (`sketch-*.png`)

## Ver localmente
```bash
python3 -m http.server 8000
# abra http://localhost:8000
```

## Publicar no GitHub Pages
1. Crie um repositório no GitHub e suba estes arquivos (`index.html` na raiz).
2. Repositório → **Settings → Pages** → Source: **Deploy from a branch** → branch `main` / pasta `/root`.
3. Aguarde ~1 min: o site fica em `https://SEU-USUARIO.github.io/NOME-DO-REPO/`.

## ⚠️ Falta fazer (ações da equipe)
- [ ] **Vídeo conceito (≤2 min)** — substituir o bloco placeholder na seção `#video` pelo embed do YouTube ou por um `assets/video.mp4` (instruções estão nos comentários do `index.html`). *Vale 50 pts.*
- [ ] **Liberar os embeds** para renderizarem no site publicado:
  - **Figma:** abrir o arquivo → *Share* → "Anyone with the link" = **can view**.
  - **Miro:** abrir o board → *Share* → habilitar acesso por link (qualquer pessoa pode ver).
  - Enquanto não liberar, os iframes aparecem vazios, mas os botões "Abrir no Figma / Miro" funcionam.
- [ ] **Fotos reais da equipe** (opcional, pega os 5 pts igual com avatar): trocar cada `<div class="avatar">` por `<img class="avatar" src="assets/foto-XX.jpg">`.

## Links do projeto
- Protótipo (Figma): https://www.figma.com/design/WlkwUAUbbs0dsNf184dEUv
- Quadro do Design Sprint (Miro): https://miro.com/app/board/uXjVHEnk3OE=/

## Cobertura da Entrega 1 (100 pts)
| Item | Pontos | Status |
|---|---|---|
| Vídeo de conceito (≤2 min, embarcado) | 50 | ⏳ slot pronto — falta gravar/embed |
| Descrição do produto + diferenciais | 10 | ✅ |
| Artefatos do Design Sprint (mapa + esboços + storyboard) | 30 | ✅ (esboços na página; mapa+storyboard via Miro embed/link) |
| Integrantes (nome + foto) | 5 | ✅ (avatar; trocar por foto se quiser) |
| Protótipo do Figma (embarcado ou link) | 5 | ✅ |
