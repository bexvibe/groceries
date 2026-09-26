# Weekly Grocery Picker

A single-file, no-build web app for picking this week's groceries from a master list.

## Usage

Open `index.html` in any browser (double-click it, or serve the folder with any static server).

- Each page is a grocery category. Tap an item to select it for this week's shop.
- Once selected, use `−` / `+` to adjust the quantity (defaults come from the master list).
- Click **Next** to move through all categories, then **Finish** to see your list.
- The final screen shows a plain-text list, grouped by category, ready to copy and hand to a shopping assistant (e.g. Claude Code, Grokbot) to place the order.

## Editing the master list

The master list lives in the `CATEGORIES` array at the top of the `<script>` block in `index.html`. Each category has a `name` and an `items` array; each item has a `name`, default `qty`, `unit` (`ea`, `kg`, `dozen`, etc.), and an optional `note`. A category can also have a `categoryNote` shown as a banner on that page (e.g. brand guidance) and included in the final list's notes section.
