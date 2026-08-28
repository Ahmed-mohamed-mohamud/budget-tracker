# Budget Tracker — Visual Identity

A CSS-only visual redesign of the Budget Tracker built in previous weeks. No new HTML structure or functionality was added — this pass focuses entirely on color, typography, table/form styling, and the CSS box model.

## What was built

- **`index.html`** — the page structure: a hero heading, an "Add Expense" form, and an expense ledger table, each wrapped as a distinct visual card.
- **`style.css`** — all visual styling: palette, fonts, spacing, borders, and component styling.
- **`README.md`** — this file.

## Design choices

**Concept:** a physical ledger / passbook, reimagined for the screen — deep forest-green ink, a gold rule for emphasis, and monospaced figures so amounts line up the way they would in a real ledger book.

**Color palette**
| Role | Color |
|---|---|
| Page / card background | `#F4F2EA` paper, `#FFFFFF` card |
| Primary ink / headings | `#17342A`, `#123A29` |
| Accent (buttons, table header) | `#1F5C43` forest green |
| Highlight (stats, index numbers) | `#C9A648` gold |
| Delete / negative action | `#B4483A` rust |
| Borders | `#DCE4DA` hairline |

Applied consistently across the page background, headings, buttons, table headers, and alternating row tints.

**Typography**
- **Fraunces** (serif, display) — page title and card headings, for an editorial/ledger feel.
- **Inter** (sans-serif, body/UI) — labels, form fields, table text, buttons.
- **IBM Plex Mono** — all monetary figures and dates, so numbers align like a real ledger.

**Table & form styling**
- Table header uses a solid forest-green band with white uppercase text.
- Alternating row backgrounds for scanability.
- Category tags use small color-coded pills.
- Form inputs share consistent padding, border-radius, and a green focus outline.
- Buttons: solid green primary action, outlined rust "Delete" action with hover fill.

**CSS Box Model**
- Every major section (hero, form, table) is its own `.card`: consistent `padding`, `border`, `border-radius`, and `margin`/`gap` spacing between cards.
- `border-collapse` keeps table borders clean; cell `padding` gives the ledger room to breathe.
- A `card-heading` uses `padding-bottom` + `border-bottom` to visually separate the heading from its content.

## How to view it

Open `index.html` directly in a browser — no build step or dependencies beyond the Google Fonts CDN link already included in the `<head>`.
