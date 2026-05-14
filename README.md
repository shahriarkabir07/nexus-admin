# NexusAdmin — Dark Modern Admin Dashboard

A sleek, fully responsive **Admin Dashboard UI** built with pure HTML5 and CSS3. No frameworks, no JavaScript dependencies — just clean, modern front-end code.



---

## ✨ Features

- **Dark modern theme** with a deep navy/charcoal color palette
- **Responsive layout** — works on desktop, tablet, and mobile
- **Sidebar navigation** with active states, badges, and user profile
- **KPI metric cards** with inline sparkline SVG graphs and trend badges
- **Bar chart** for monthly revenue with hover interactions (pure CSS)
- **Donut chart** for traffic source breakdown (pure SVG)
- **Orders table** with avatar initials, status badges, and row hover effects
- Zero external JS dependencies — everything runs with HTML + CSS only

---

## 📁 Project Structure

```
admin-dashboard/
├── index.html      # Main dashboard page
├── style.css       # All styles, tokens, and responsive rules
└── README.md       # This file
```

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/admin-dashboard.git
cd admin-dashboard
```

### 2. Open in your browser

No build step required. Just open `index.html` directly:

```bash
# macOS
open index.html

# Windows
start index.html

# Linux
xdg-open index.html
```

Or use a local dev server for live reload:

```bash
# Using VS Code Live Server extension (recommended)
# Right-click index.html → "Open with Live Server"

# Using Python
python -m http.server 8000
# Then visit http://localhost:8000
```

---

## 🎨 Design Tokens

All colors and layout values are defined as CSS custom properties in `:root` inside `style.css`, making it easy to customize:

| Token | Value | Usage |
|-------|-------|-------|
| `--bg-base` | `#0d0f17` | Page background |
| `--bg-surface` | `#131621` | Sidebar background |
| `--bg-card` | `#181c2a` | Card backgrounds |
| `--accent` | `#a78bfa` | Primary violet accent |
| `--accent-blue` | `#38bdf8` | Sky blue accent |
| `--accent-green` | `#34d399` | Emerald green accent |
| `--accent-warn` | `#fbbf24` | Amber warning |
| `--accent-red` | `#f87171` | Red error |
| `--font` | `Syne` | Display/UI font |
| `--mono` | `DM Mono` | Monospace font |

---

## 📐 Responsive Breakpoints

| Breakpoint | Layout |
|------------|--------|
| `> 1200px` | 4-column KPI grid, side-by-side charts |
| `≤ 1200px` | 2-column KPI grid, stacked charts |
| `≤ 768px` | Sidebar hidden, single-column layout |
| `≤ 480px` | Single-column KPI grid |

---

## 🧩 Components

### KPI Cards
Metric summary cards with:
- Percentage change badge (green = positive, red = negative)
- Sparkline SVG mini-chart in the bottom-right corner
- Hover border highlight

### Bar Chart
CSS-only bar chart with:
- `--h` CSS variable controlling bar height per column
- Tooltip labels appearing on hover/active
- Active bar highlighted with accent color
- Dashed baseline rule

### Donut Chart
SVG-based donut chart using `stroke-dasharray` / `stroke-dashoffset` technique with a centered value label and a color legend.

### Orders Table
Responsive data table with:
- Inline avatar initials colored per user
- Status badges (Completed / Pending / Failed)
- Row hover highlights

---

## 🔧 Customisation Tips

**Change the accent color** — update `--accent` in `:root`:
```css
:root {
  --accent: #f472b6; /* pink theme */
}
```

**Add a new nav item** — copy a `.nav-item` block in `index.html` and swap the SVG icon.

**Add a new KPI card** — copy a `.kpi-card` div and update the label, value, sub-text, and sparkline points.

---

## 🌐 Browser Support

| Browser | Support |
|---------|---------|
| Chrome 90+ | ✅ Full |
| Firefox 88+ | ✅ Full |
| Safari 14+ | ✅ Full |
| Edge 90+ | ✅ Full |

> **Note:** `color-mix()` (used for table avatar tints) requires Chrome 111+, Firefox 113+, Safari 16.2+. A fallback solid color is used in older browsers.

---



---

## 👨‍💻 Author

**Shahriar Kabir**
- GitHub: [@shahriar-kabir](https://github.com/shahriar-kabir)

---

## 🙌 Credits

- Fonts: [Syne](https://fonts.google.com/specimen/Syne) & [DM Mono](https://fonts.google.com/specimen/DM+Mono) via Google Fonts
- Icons: Inline SVG (no external icon library required)

---

*Built with ❤️ by [Shahriar Kabir](https://github.com/shahriar-kabir) using pure HTML & CSS — no frameworks, no nonsense.*
