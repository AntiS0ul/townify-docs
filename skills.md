/* ===========================================================
   TownifyMC Guide — custom theming
   Layered on top of Material's amber palette.
   =========================================================== */

:root {
  --md-primary-fg-color:        #d4a017;
  --md-primary-fg-color--light: #e6b800;
  --md-primary-fg-color--dark:  #a87b0a;
  --md-accent-fg-color:         #e8851a;
}

/* Slightly warmer dark slate so it reads as "evening survival server" */
[data-md-color-scheme="slate"] {
  --md-default-bg-color: hsl(232, 15%, 12%);
  --md-code-bg-color:    hsl(232, 15%, 16%);
}

/* Tighten the hero headings a touch */
.md-typeset h1 {
  font-weight: 700;
  letter-spacing: -0.01em;
}

/* Rank ladder & price tables: make them feel like a game UI */
.md-typeset table:not([class]) {
  font-size: 0.78rem;
}
.md-typeset table:not([class]) th {
  background-color: var(--md-primary-fg-color--dark);
  color: #fff;
}

/* Currency / cost chips you can drop inline with {.chip} on a span */
.chip {
  display: inline-block;
  padding: 0.05em 0.5em;
  border-radius: 0.6em;
  font-weight: 600;
  font-size: 0.85em;
  line-height: 1.5;
  white-space: nowrap;
}
.chip.money  { background: rgba(76, 175, 80, 0.18);  color: #4caf50; }
.chip.gems   { background: rgba(156, 39, 176, 0.18); color: #ce93d8; }
.chip.points { background: rgba(33, 150, 243, 0.18); color: #64b5f6; }

/* Make the "grid cards" on landing pages a little punchier */
.md-typeset .grid.cards > ul > li {
  border-radius: 0.6rem;
  transition: border-color 200ms, box-shadow 200ms;
}
.md-typeset .grid.cards > ul > li:hover {
  border-color: var(--md-accent-fg-color);
  box-shadow: 0 0 0 1px var(--md-accent-fg-color);
}

/* Rank tier color hints for the ladder page (matches in-game tag colors) */
.tier-common    { color: #bdbdbd; font-weight: 600; }
.tier-uncommon  { color: #66bb6a; font-weight: 600; }
.tier-rare      { color: #4dd0e1; font-weight: 600; }
.tier-epic      { color: #5c6bc0; font-weight: 600; }
.tier-legendary { color: #ba68c8; font-weight: 600; }
.tier-royal     { color: #ffb300; font-weight: 600; }
.tier-celestial { color: #ffee58; font-weight: 700; }
