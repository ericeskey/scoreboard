# Claude Design Prompt — Scoreboard microsite V3 → V4 (Harsh's voice threaded through)

**Target:** the existing live project behind **scoreboard.darkhorse.works** (built for Matt Becker, Teleflex). Same Claude Design project that also holds the one-pager PDF.
**Version bump:** footer currently reads **V3 · 2026**. This pass ships **V4**. Update the footer/version string everywhere it renders.
**Spine (unchanged):** 01 Engage · 02 Listen · 03 Frame · 04 Crux · 05 Envision · 06 Commit · 07 Close · 08 Kickoff · (Essays + Case room off-spine).

**Why V4 exists, in one line:** Matt recovered Harsh Kachhy's own January 2025 email and KPI spreadsheet, the document that *originated* this whole scoreboard 18 months ago. V4 makes Harsh's voice visible throughout so that when he reads the site (he is the sponsor, and a rescheduled review with him is imminent), he recognizes the design as the matured form of his own 2025 idea, not a vendor's proposal dropped on him.

---

## FILES TO PROVIDE TO CLAUDE DESIGN
1. **The existing scoreboard project source** (behind scoreboard.darkhorse.works) — reuse the design system exactly: dark theme, Inter / Instrument Serif / JetBrains Mono, accent color, card grammar, the "This lands / Not quite" reaction model, the session/record mechanism, nav + prev/next flow. Nothing should look new; the site should look like it grew.
2. **The one-pager PDF** (already in this project) — `Sustaining portfolio scoreboard, outcome first.pdf`, refreshed in the companion prompt. V4 wires it as a downloadable Tl;dr (see §D).
3. This prompt.

**Do NOT touch:** existing recorded reactions / localStorage session state. Preserve all of it. Keep every existing URL working.

---

## PROMPT (paste into Claude Design)

You are evolving an existing, live personalized microsite, scoreboard.darkhorse.works, built for one reader: Matt Becker, a senior sustaining-engineering portfolio leader at Teleflex. Study the current project source first. This is a small, surgical version bump, V3 to V4. Keep the design system, spine, card grammar, reaction model, and session record exactly as they are. Do not restructure the spine. Make only the four changes below, then update the version string to V4.

The purpose of V4: thread the voice of Harsh Kachhy through the site. Harsh is Matt's sponsor and the executive who will read this. In January 2025 Harsh sent Matt a spreadsheet of recommended sustaining KPIs with a written charge to build exactly this scoreboard. That document is the true headwater of everything on the site. V4 should make a cold-reading Harsh feel his own prior thinking reflected back to him, so blessing the design reads as recognizing his own idea.

Every quote attributed to Harsh below is verbatim from his January 3, 2025 email and spreadsheet. Do not paraphrase his quoted words. No em-dashes anywhere. No pricing, rate, or contract language anywhere. No DHW-internal vocabulary.

### CHANGE A — 01 Engage: add a "Where this began" element

The Engage page already tells the recent origin (June 16, the pause, Harsh accepting all five recommendations). Add one new element ABOVE or immediately after that recommendations block, a distinct panel titled **"Where this began."** It reaches back further than the pause story, to the original charge. Keep it short and quietly authoritative, in the existing essay voice. Content:

> **Where this began**
> This scoreboard is not a new idea. In January 2025, Harsh asked for it directly.
>
> *"Please take the lead here and convert to the most succinct and actionable views. This should serve as the basis of future monthly Enterprise Reviews. Create baseline views and refine with sustaining leads as needed."*
> — Harsh Kachhy, January 3, 2025
>
> Everything that follows is the disciplined, evidence-tested form of that charge: the measures Harsh named, mapped to the decisions they change, tested against the data that actually exists today.

Style the quote in the same treatment the site uses for attributed voices. This panel is reference, not reactable (match how the existing "five recommendations, as accepted" block reads).

### CHANGE B — 02 Listen: upgrade Harsh's card to his written charge

Harsh already appears on the Listen page as an attributed voice (currently rendered from the "Kachhy" listening card). Upgrade that card so its body carries his actual written words from the recovered email, and its expandable context notes that this is the original January 2025 charge that the current work fulfills. Keep the card reactable, keep the existing attribution treatment. Card body (verbatim quote):

> *"Please take the lead here and convert to the most succinct and actionable views. This should serve as the basis of future monthly Enterprise Reviews."*

Expand/more-context line:
> Harsh's January 3, 2025 email to Matt (cc Jake Newman), attaching his recommended sustaining KPIs. It set the register the quarterly still aims for: succinct, actionable, decision-driving. His own numeric targets from that file appear on the measures below.

Do not disturb the other Listen cards or their recorded reactions.

### CHANGE C — the Decisions and Measures pages: light provenance + Harsh's verbatim targets

Two surfaces carry the substance Harsh cares about: the **eight decisions** (08 Kickoff, "The decisions the room owns") and the **twelve measures** (05 Envision, State A, the KPI cards). On these:

1. **Provenance marker.** On each measure that traces to Harsh's 2025 recommendations, add a small, unobtrusive tag or footline reading **"Traces to Harsh's Jan-2025 recommendation."** Use the same visual weight as the existing [Now] / [Step] / [Build] tags; do not shout. Apply it to these measures: Portfolio completion velocity; Aging and backlog trend; Cycle time by project class; At-risk project exposure; Supplier and obsolescence exposure; Compliance-linked risk; Reactive vs. proactive load split; Margin-improvement pipeline; Realized margin improvement; Cost of sustaining and revenue at risk. Do NOT tag **Recurrence rate** — instead give it a one-word marker **"New"** with an expand line: *"A DHW addition, not in the 2025 set: a project that comes back was never truly closed. A leading quality signal."*

2. **Harsh's own targets, verbatim.** Two measures have hard numeric targets that are Harsh's own words from the 2025 file. Surface them on the relevant cards as his stated bars:
   - Portfolio completion velocity: **"Improve ratio of completed to active projects, 6% to 10%."** (Harsh, Jan 2025)
   - Cycle time / on-time completion: **"Improve on-time completion, 40% to 60%, on A/B/C projects."** (Harsh, Jan 2025)
   Render these as quoted target lines attributed to Harsh, so the bar the measure is judged against is visibly his.

3. **The reachable-now correction.** Make sure the "reachable now, from data in hand" set reads correctly as **two measures in Direction & Delivery (completion velocity, aging and backlog) plus two in Risk**, not four within a single category. If the current V3 layout can be misread as four-in-one-category, fix the grouping so the 2+2-across-categories split is unambiguous.

On the eight decision cards, no per-card quotes are needed, but add one framing line at the top of the decisions section: **"These are the decisions Harsh's 2025 'Big Questions' were always driving at, made explicit."** Keep the decisions rendered as DRAFT/for-correction as they are today.

### CHANGE D — wire the one-pager as a downloadable Tl;dr

The refreshed one-pager PDF lives in this same project. Add a **"Download the one-page Tl;dr"** affordance (a clean download button/link in the site's existing button style) in two places: on **01 Engage** (near the "Where this began" panel or the intro) and on **06 Commit**. Label it plainly, e.g. *"The whole thing on one page (PDF)."* It links to / serves the project's one-pager PDF. No new page; just the download affordance. If the build serves static assets from a known path, place the PDF there and link it; note in your return which path you used.

### After the four changes
- Bump the version string to **V4** wherever the footer/version renders (currently V3 · 2026 → V4 · 2026, keep the site's existing format).
- Update nothing else in the spine, copy, or interaction model.

## GUARDRAILS (unchanged from prior passes)
- No em-dashes. No pricing / rate / fee / contract language (grep the build for `$`, "fee", "rate", "price").
- Verbatim quotes stay verbatim; never paraphrase Harsh's or any colleague's quoted words.
- No DHW-internal vocabulary (no "crux", "FLS", "trust stage", frame slugs, "terrain memo", encounter references).
- Client's own tool names are fine (Power BI, Planview, SAP, Smartsheet, SharePoint, etc.).
- Preserve all existing recorded reactions and the session record across every page.
- Names and roles rendered respectfully and exactly; no editorializing about any person.

## POST-BUILD VERIFICATION CHECKLIST
1. Footer reads V4 everywhere; no V3 left.
2. 01 Engage has a "Where this began" panel with Harsh's verbatim Jan-2025 charge.
3. 02 Listen's Harsh card carries his written charge verbatim and expands to the Jan-2025 context; other Listen cards + their reactions untouched.
4. Measures page: provenance tags on the ten traced measures; "New" marker + expand on Recurrence rate; Harsh's 6%→10% and 40%→60% targets shown as his quoted bars; reachable-now reads as 2 Direction + 2 Risk.
5. Decisions section carries the "Harsh's Big Questions, made explicit" framing line; still renders as draft/for-correction.
6. "Download the one-page Tl;dr" button works on 01 Engage and 06 Commit and serves the PDF.
7. grep the build: zero `$`/fee/rate/price, zero em-dashes, zero internal vocabulary.
8. All existing URLs and recorded reactions survive; mobile rendering of new panel + tags is clean before sharing with Matt.
9. Return the list of exactly which files you modified and the asset path used for the PDF.
