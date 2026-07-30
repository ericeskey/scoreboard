# Claude Design Prompt — "07 Kickoff" page(s) for scoreboard.darkhorse.works

**Scope: ADD a new section to the existing live site. Do not modify the existing ladder pages (01 Listen through 06 Close) except the single nav addition. Preserve the site's visual system, card grammar, reaction storage (do not touch existing localStorage state), and all existing URLs.**

## What this addition is

The engagement has verbally closed; the SOW is in co-edit. This page moves the site from selling surface to WORKING surface: the Phase 1 kickoff plan, walked through live with Matt on the Thursday co-edit call. Tone shift from the ladder pages: less persuasion, more logistics-with-reasons. It should feel like the first page of the engagement, not the last page of the pitch.

## Navigation

Add one item to the spine after the existing final page: **"07 Kickoff"**. If the build works better as one page with four anchored sections, do that; if as a parent page with three subpages, that also works. Prefer one scrolling page: this gets walked top-to-bottom on a call.

## Page structure (four sections, in this order)

### Section 1: "The first three days" (from run-of-show, file 22)
Render the Ireland kickoff agenda as a three-column day layout (Day 1 Terrain / Day 2 Snapshots at the source / Day 3 First-pass mapping, marked optional-but-recommended). Each day: morning block, afternoon block, and a one-line output statement styled distinctly (these are the "what comes out" lines; Matt asked for exactly this shape). Include the "Before we arrive" items as a short checklist above the days. Practical notes (travel per SOW, day-3 fallback) as a muted footnote row. Include the proposed timing: week of August 10, at the command center.

### Section 2: "What we need in hand" (from snapshot request list, file 19)
The eight snapshot requests as a numbered checklist-style card grid, each card: item name, one-line description, likely owner, and an empty status affordance (requested / in flight / received: static labels are fine, no backend). Ground-rules strip beneath, verbatim from the file's four ground rules: one-time snapshots not feeds; as-is beats cleaned-up (the warts are data); confidentiality terms; blocked extracts are findings too. Item 8 (the 20-project trace sample) gets slight visual emphasis: it is the financial-path test.

### Section 3: "The decisions the room owns" (from decision inventory, file 20)
The eight draft decisions as reactable cards (same affirm/adjust interaction grammar as the Listen page if cheap to reuse; otherwise plain cards with room for penciled notes). Frame line above the grid, verbatim: "Draft, for correction. Every candidate measure gets mapped against this list: a measure that would not change any of these decisions is out, no matter how good its data." Include the short "What the room does NOT own" list as a muted companion card: it protects BU leads' territory in writing. Do NOT include the parenthetical provenance notes from the file (the reconciliation-gap and Lidocaine references stay off this page; they are conversation material).

### Section 4: "How we'll work" (rhythm + posture)
Three compact cards:
1. **The window.** The standing three-way overlap: 6-9 am Arizona / 9-noon Pennsylvania / 2-5 pm Ireland. Render as a simple three-timezone bar visual if cheap.
2. **The loop.** Snapshot → mockup → react → adjust; one structured feedback cycle per the SOW; weekly working session, 60 minutes early weeks settling to 30.
3. **Built once.** One sentence: "Discovery runs on snapshots so that what gets built at the end gets built once, from a confirmed baseline." (This is the Andreas-posture sentence; it belongs on the page he may eventually see.)

## Hard rules

- **No pricing anywhere.**
- **No em-dashes.**
- **No names except Matt and Eric.** Andreas appears as "the PBI developer" / "the command center team." The 15 field questions (file 21) are NOT on this page in any form: they are a working paper, not a site artifact.
- No DHW-internal vocabulary (no "crux," "breadcrumb," "terrain memo" is acceptable as "systems map").
- The decision inventory renders as DRAFT, visually: this page invites correction, and looking finished would defeat it.
- Existing pages, reactions, and URLs untouched; verify the Listen page reaction state survives the deploy.

## Post-build verification checklist

1. grep built page for $ amounts, "fee", "rate", em-dashes: expect zero.
2. Spot-check: the three-day agenda's output lines present; eight snapshot cards; eight decision cards + NOT-owned card; the timezone window correct (6-9 / 9-noon / 2-5).
3. Confirm 01-06 pages unchanged and reactions persist.
4. Confirm "07 Kickoff" reachable from the spine nav.

## Files provided with this prompt

- 22_kickoff_run_of_show.md (section 1 source)
- 19_snapshot_request_list.md (section 2 source)
- 20_decision_inventory.md (section 3 source; strip provenance parentheticals)
- Existing site source (visual system + nav)
