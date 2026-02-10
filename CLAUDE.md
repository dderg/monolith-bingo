# Monolith Bingo

Single-page bingo game themed around common newcomer choices in the Monolith 3D printer community.

## Structure

- `index.html` — the entire app (HTML + CSS + JS, no build step)
- Deployed via GitHub Pages (`.github/workflows/pages.yml`)

## How it works

- `ALL_ITEMS` array holds the bingo square texts (exactly 24 needed for a 5x5 grid with a free center)
- On load and on shuffle, 24 items are randomly arranged into the grid with a free space at center (index 12)
- Clicking a cell toggles its stamped state; bingo detection checks all rows, columns, and diagonals

## Editing cards

Add or remove entries in the `ALL_ITEMS` array in `index.html`. Keep the count at 24 for a full board. If more than 24 items exist, 24 are randomly selected each shuffle.
