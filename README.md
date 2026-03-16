# 🎲 Ludothèque — Board Game Rules

**Live site**: https://akais315.github.io/boardgames/

A mobile-friendly board game rules library hosted on GitHub Pages.  
Designed for guests: scan a QR code on the box → read the rules on their phone.

---

## 📁 Structure

```
boardgames/
├── index.html          ← Game library (filterable)
├── README.md
└── rules/
    └── codenames.html  ← One file per game
```

## ➕ Adding a game

1. **Add a card** in `index.html` — copy an existing `<a class="card">` block and fill in the data attributes
2. **Create a rules file** in `rules/yourgame.html` — copy `rules/codenames.html` as template
3. Set `data-rules="true"` on the card and update `href` to point to the new file
4. Commit & push — GitHub Pages deploys in ~1 minute

## 🏷️ Available tags

| Tag | Usage |
|-----|-------|
| `coop` | Cooperative game |
| `compet` | Competitive |
| `team` | Team-based |
| `family` | Family-friendly |
| `strategy` | Strategy heavy |
| `party` | Party game |
| `words` | Word game |
| `deduct` | Deduction/hidden role |

## 🖼️ Cover images

Drop game cover images in a `covers/` folder and reference them in the card:
```html
<img class="card-cover" src="../covers/codenames.jpg" alt="Codenames">
```
Recommended size: 300×200px or any 3:2 ratio.
