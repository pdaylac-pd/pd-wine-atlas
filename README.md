# PD | Wine Atlas

Dashboard pessoal de estudos de vinho. Consulta rápida de **regiões, uvas e curiosidades** organizado por país e sub-região, com mapas Wine Folly originais.

**🍷 Live:** `https://<seu-usuario>.github.io/pd-wine-atlas/`

---

## Conteúdo atual (v1.0)

### Países (6)
- 🇦🇺 Austrália
- 🇪🇸 Espanha
- 🇺🇸 Estados Unidos
- 🇫🇷 França
- 🇮🇹 Itália
- 🇳🇿 Nova Zelândia

### Deep dives (6)
- 🍇 Napa Valley (dentro dos EUA)
- 🍇 Sonoma County (dentro dos EUA)
- 🍷 Borgonha (dentro da França)
- 🥂 Champagne (dentro da França)
- 🏰 Loire (dentro da França)
- 🍇 Piemonte (dentro da Itália)

### Catálogo de uvas (9)
Cabernet Sauvignon · Chardonnay · Gamay · Merlot · Pinot Noir · Riesling · Sauvignon Blanc · Syrah/Shiraz · Zinfandel

Cada uva inclui: berço, perfil sensorial (corpo, taninos, acidez), aromas característicos, 6 países/regiões onde brilha (com **selo BENCHMARK** no berço de origem) e pareamento.

---

## Stack técnica

- **HTML único** (`index.html`) — sem build, sem dependências locais
- **Tailwind CSS** via CDN
- **Chart.js** via CDN (gráficos de produção, composição, pirâmides de classificação)
- **Tipografia:** Playfair Display + Inter (Google Fonts)
- **Mapas:** PNG/JPG Wine Folly hospedados em `images/` + fallback automático para CDN Wine Folly

Total: **40+ páginas**, **22 gráficos**, **9 uvas catalogadas**, **18 mapas Wine Folly**.

---

## Estrutura de pastas

```
pd-wine-atlas/
├── index.html
├── README.md
├── .gitignore
└── images/
    ├── australia-wine-regions.png
    ├── burgundy-beaujolais-map.jpg
    ├── burgundy-chablis-map.jpg
    ├── burgundy-cote-chalonnaise-map.jpg
    ├── burgundy-cote-de-beaune-map.jpg
    ├── burgundy-cote-de-nuits-map.jpg
    ├── burgundy-maconnais-map.jpg
    ├── burgundy-map.jpg
    ├── champagne-map.jpg
    ├── italy-classifications.png
    ├── italy-label.png
    ├── italy-puglia-map.jpg
    ├── italy-wine-regions.jpg
    ├── new-zealand-map.jpg
    ├── piedmont-map.jpg
    ├── piedmont-nebbiolo-map.jpg
    ├── spain-wine-regions.jpg
    └── usa-wine-regions.png
```

---

## 🚀 Como publicar no GitHub Pages (3 passos)

### 1. Criar o repositório no GitHub

**Opção A — via GitHub CLI (mais rápido):**

```bash
cd ~/path/para/pd-wine-atlas
gh repo create pd-wine-atlas --public --source=. --remote=origin --push
```

**Opção B — via web (manual):**

1. Vá em [github.com/new](https://github.com/new)
2. Repository name: `pd-wine-atlas`
3. Public · sem README, .gitignore ou LICENSE (já existem)
4. Clique em **Create repository**
5. Copie a URL do repo

### 2. Push do código

```bash
cd ~/path/para/pd-wine-atlas
git init
git add .
git commit -m "v1.0 — 6 países, 6 deep dives, 9 uvas, 18 mapas"
git branch -M main
git remote add origin https://github.com/<seu-usuario>/pd-wine-atlas.git
git push -u origin main
```

### 3. Ativar GitHub Pages

1. No repo, vá em **Settings → Pages**
2. **Source:** Deploy from a branch
3. **Branch:** `main` · **Folder:** `/ (root)`
4. **Save**
5. Em 1–2 minutos, acesse: `https://<seu-usuario>.github.io/pd-wine-atlas/`

---

## Roadmap

- [x] v0.1 — EUA + Napa Valley
- [x] v0.2 — Austrália
- [x] v0.3 — França + Borgonha + Beaujolais
- [x] v0.4 — Sub-regiões Borgonha + Sonoma
- [x] v0.5 — Loire + Champagne dentro da França
- [x] v0.6 — Nova Zelândia
- [x] v0.7 — Espanha
- [x] v0.8 — Itália + Piemonte
- [x] **v1.0 — Publicação GitHub Pages**
- [ ] v1.1 — Toscana (dentro da Itália) + materiais PDF
- [ ] v1.2 — Portugal (Douro, Alentejo)
- [ ] v1.3 — Bordeaux + Rhône (dentro da França)
- [ ] v1.4 — Alemanha (Mosel) + Áustria
- [ ] v1.5 — Hemisfério Sul (Chile, Argentina, África do Sul)
- [ ] v2.0 — Busca global + filtro cruzado + sistema de notas pessoais

---

## Fontes

- [Wine Folly — Wine Regions](https://winefolly.com/wine-regions/)
- [Wine Folly — Burgundy Guide](https://winefolly.com/deep-dive/guide-to-burgundy-wine-with-maps/)
- [Wine Folly — Beaujolais Guide](https://winefolly.com/deep-dive/beaujolais-wine-region-map/)
- [Wine Folly — Loire Valley Guide](https://winefolly.com/deep-dive/loire-valley-wine-guide/)
- [Wine Folly — Champagne Guide](https://winefolly.com/deep-dive/how-to-choose-champagne/)
- [Wine Folly — Piedmont Guide](https://winefolly.com/deep-dive/piedmont-wine-guide/)
- [Wine Folly — Spain Map](https://winefolly.com/deep-dive/map-of-spain-wine-regions/)
- [Wine Folly — Italy](https://winefolly.com/wine-regions/italy/)
- [Wine Folly — Napa Valley Guide](https://napa.guides.winefolly.com/)

---

## Licença

MIT (código). Mapas e marcas são propriedade de Wine Folly e referenciados para fins de estudo pessoal.

Construído por **Patrick Daylac** · 2026
