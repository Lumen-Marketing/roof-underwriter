# Roof Underwriter

Internal roofing estimator: builds a labor + material cost sheet per roof system
(shingle / tile / foam / metal), applies sales tax and commission, and shows net
profit, margin health and a payment schedule.

## Use

Open the page. Pick a roof system, set squares, fill quantities, enter the client
quote. The "Price to a margin" slider back-solves the quote needed for a target
net margin.

- **Admin** unlocks the locked unit prices. `ADMIN_PIN` in `index.html` is empty,
  so the button unlocks instantly. Set it to a code to require one from reps.
- **Second system** appends a whole second system as an add-on group.
- Saved deals are stored in the browser via `localStorage`, so they are per-device
  and per-browser. Clearing site data clears them.

## Editing

Everything is one self-contained `index.html`. Default rates live in the
`SYSTEMS` object; `TAX_RATE` sits just above it.
