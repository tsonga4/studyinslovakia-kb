# Knowledge base — faculty directory (home page plan)

Tracks the faculties shown on the KB home page (`docs/index.md`), their status,
and the section each one links to. This file lives in the repo root only — it is
**not** part of the published site.

## Working rules

- Faculty and university names are kept **verbatim** as provided by the user
  (including current typos / capitalisation). Do not "correct" them unless the
  user explicitly asks.
- Comenius University appears as **two** separate entries (Bratislava and
  Martin), exactly as the user listed them.
- Only add content the user provides. Nothing is fabricated. See the memory note
  `no-fabricated-content`.

## Faculties & status

Status legend: ✅ done (has a guide) · ⏳ coming soon (listed, no content yet)

### University of Pavol Jozef Safarik
- Faculty of medicine — ✅ **done** — section `docs/lf-upjs/` → `lf-upjs/index.md`

### Comenius University in Bratislava
- Faculty of medicine — ⏳ coming soon

### Comenius University in Martin
- Jessenius Faculty of medicine — ⏳ coming soon

### Technical University in Kosice
- Faculty of Economics — ⏳ coming soon
- Faculty of Electrical engineering and Informatics — ⏳ coming soon
- Faculty of Mechanical Engineering — ⏳ coming soon
- Faculty of Aeronautics — ⏳ coming soon

### Slovak Technical University in Bratislava
- Faculty of Mechanical engineering — ⏳ coming soon
- Faculty of Civil engineering — ⏳ coming soon
- Faculty of Chemical and food technology — ⏳ coming soon
- Faculty of electrical enginering and Information technology — ⏳ coming soon

### Bratislava University of Economics and Management
- (standalone university, no separate faculty) — ⏳ coming soon

### Economic University in Bratislava
- (standalone university, no separate faculty) — ⏳ coming soon

## How to add a faculty's content

When the user provides material for a faculty:

1. Create pages under `docs/<slug>/` from the user's text (tables, checklists,
   admonitions — no invented content).
2. Add the new section to `nav:` in `mkdocs.yml`.
3. On `docs/index.md`, change that faculty's card from `_Coming soon_` to a link
   (`[:octicons-arrow-right-24: Open guide](<slug>/index.md)`).
4. Update the status in this file (⏳ → ✅) and record the slug.
