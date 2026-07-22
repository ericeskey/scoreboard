# Claude Design Prompt — Restructure scoreboard.darkhorse.works to the working-session ladder (V3)

**Purpose:** evolve the Matt Becker microsite from the current essay-led spine (Engage → Listen → Bridge → Essay I → Essay II → Blueprint → Close) into a **working-session ladder** modeled on psi.darkhorse.works/PSI Andover Working Session: **Listen → Frame → Crux → Envision → Commit**, where affirmed reactions climb the trust ladder toward a commitment draft. Everything Matt has already reacted to is preserved; the essays and case room move off-spine as reference.

---

## FILES TO PROVIDE TO CLAUDE DESIGN

**Essential (design + structure references):**
1. **The existing scoreboard microsite source** — full project behind scoreboard.darkhorse.works. Claude must reuse the design system (dark theme, Inter/Instrument Serif/JetBrains Mono, accent color, card components, affirm/flag "This lands / Not quite" interaction, the reaction record/session mechanism) rather than invent anything new. This is also the source of the existing Blueprint page content (agenda + KPI cards) that gets absorbed into the new Envision page.
2. **The PSI working-session page source** — the file behind psi.darkhorse.works/PSI Andover Working Session.dc.html. This is the *structural* reference: the ladder page flow, how listening cards lead to framing cards lead to crux surfaces lead to envisioned states lead to a commit draft, and how the end-of-session record compiles what was affirmed. Match the scoreboard site's VISUAL system, but the PSI page's STRUCTURAL logic.

**Content sources (the five new/rebuilt pages — provided as card-shaped markdown with CARD/BODY/EXPAND markers):**
3. `microsite_src/listen.md` — 12 attributed listening cards (replaces the current 8-card Listen readback; the original 8 cards' affirmed reactions should be preserved in the record, and if feasible noted as "previously affirmed" where content carries over)
4. `microsite_src/frame.md` — 8 framing cards
5. `microsite_src/crux.md` — diagnosis panel + 5 comparable crux candidates + the stated crux
6. `microsite_src/envision.md` — three states (A: first quarterly EPR, absorbing the existing Blueprint agenda + KPI cards and their reaction state; B: the system a year out; C: the work between)
7. `microsite_src/commit.md` — the commitment draft (6 cards, NO pricing anywhere)

**Do NOT provide:** any DHW-internal files (pricing rationale, audits, assumption stacks, crux analyses in their internal form, the scoreboard ledger, team briefings). The `microsite_src/` files are the client-ready versions; use only those.

---

## PROMPT (paste into Claude Design)

You are restructuring an existing, live personalized microsite — scoreboard.darkhorse.works — built for one reader: Matt Becker, a senior sustaining-engineering portfolio leader at a large medical-device company. I am giving you (a) the current site source and (b) a second site's working-session page as a structural reference. Study both first.

**Design system: unchanged.** Keep the current site's dark theme, typography (Inter / Instrument Serif / JetBrains Mono), accent color, card components, motion, nav treatment, and especially the existing "This lands / Not quite" reaction model and the session record mechanism. Nothing should look new; everything should look like the site grew.

**Structure: evolve to the working-session ladder.** The current spine (01 Engage → 02 Listen → 03 Bridge → 04 Essay I → 05 Essay II → 06 Blueprint → 07 Close) becomes:

- **01 Listen** — rebuilt from `listen.md`: twelve cards, each attributed to a named person in Matt's organization, each with a short body and an expandable fuller context. This page's job: everyone whose words are on it should feel accurately heard when Matt shows it to them. Keep every card reactable.
- **02 Frame** — new page from `frame.md`: eight candidate framings of the work, each tracing to voices on the Listen page. Reactable cards with expandable context.
- **03 Crux** — new page from `crux.md`: a diagnosis panel, then five candidate cruxes rendered as comparable surfaces (the reader should be able to weigh them against each other — consider a consistent card layout with an explicit critique line per candidate), closing with the crux stated once. Reactable.
- **04 Envision** — rebuilt from `envision.md`, ABSORBING the current Blueprint page: State A (the first quarterly EPR) carries the existing agenda-beat cards and the twelve KPI cards with their current reaction behavior and any recorded reactions preserved; State B (the system a year out); State C (the work between). The [Now]/[Build] tag treatment and financial-as-destination framing from the existing Blueprint page carry over unchanged.
- **05 Commit** — new page from `commit.md`: the commitment draft. Six cards: the object, the shape, what it does not include, what success looks like, the immediate next step, the standing record. This page must contain NO pricing, no rate language, no contract terms. It proposes a bounded first engagement and a 30-minute shape conversation.
- **06 Close** — keep the existing close (standing offer + the record), updated so the record now compiles reactions across all five ladder pages.
- **Essays and Case room move off-spine:** keep them accessible from the nav or a "reference" area (like the existing case room treatment) with their existing URLs working. They are the intellectual foundation; the ladder is now the working surface.

**Card interaction pattern (all five ladder pages):** each card = attribution/title + 1–3 sentence body + expandable "more context" section (the EXPAND content in the markdown). Expansion should be inline and unintrusive (collapse/expand, no modals). Every card keeps the "This lands / Not quite" reactions feeding the session record. Where a page has free-text response boxes in the current site ("Add what this sketch missed"), keep one per page.

**Attribution handling (important):** the Listen page names real colleagues (Harsh Kachhy, Ron Aplin, Matthew James, Sara Eslinger, Andrej Baranek, Nishith Desai, Cory O'Rorke, Ken Whitley, Jake Newman, Hannah Papes, and others). Render names and roles respectfully and exactly as given in `listen.md`. Do not editorialize about any person. Every quote is verbatim from the provided files; do not paraphrase quoted material.

**Tone and guardrails:** generous, precise, collaborative — the voice of the existing essays. No sales language, no pricing, no vendor/tool names beyond those the client's own people named (Power BI, Smartsheet, SharePoint, Planview, SAP, monday.com, Microsoft Lists are all fine — they are the client's own vocabulary). The reader should feel the thinking is organized FROM his organization's own words, and that reacting to it is the first pass of the work.

**Progress/trust mechanics:** if the PSI structural reference uses a visible sense of progression through the ladder (step indicators, "continue" affordances compiling toward the commit page), reproduce that spirit: the reader should feel each page's affirmations carrying forward, with the Commit page reading as the natural landing of everything affirmed above it.

**Technical:** match the existing build and file conventions; update nav, routing, and prev/next flow to the new spine; preserve the existing session/record mechanism and extend it across the new pages; keep existing essay/case-room URLs working; responsive; match existing accessibility patterns. Return the new/changed files and list exactly which existing files you modified.

---

## AFTER CLAUDE RETURNS — verification checklist

- Spine renders: Listen → Frame → Crux → Envision → Commit → Close; essays + case room reachable off-spine at working URLs.
- Existing Blueprint reactions (if any were recorded) survive inside Envision State A; KPI cards keep [Now]/[Build] treatment.
- Every card expands/collapses; reactions on all five pages flow into one record; the Close page's record includes all of them.
- Names, roles, and quotes on Listen match `listen.md` exactly (spot-check Harsh Kachhy, Ron Aplin's quote, Matthew James's quote, the 24+14 numbers on Andrej's card).
- NO pricing, rate, or contract language anywhere (grep the build for $ signs and "fee"/"rate"/"price").
- No DHW-internal vocabulary leaked (no "FLS", "trust stage", "crux X2", frame slugs, or encounter-file references).
- Mobile rendering of expandable cards is usable before sharing the link with Matt.
