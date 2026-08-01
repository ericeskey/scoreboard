# Claude Design Prompt — Kickoff page UPDATE (v2 → v3) for scoreboard.darkhorse.works

**Scope: UPDATE the existing Kickoff surface of the live site, plus one footer version bump. Do not modify any other surface (Engage, Listen, Frame, Crux, Envision, Commit, Close, Bridge, Essays, Cases) except the footer. Preserve the site's visual system, card grammar, reaction storage (do not touch existing localStorage state or its KEY), and all existing URLs.**

## Why this update

The Kickoff page was drafted before the measurement design behind the workshop was finished. The engagement's evidence-first discipline is now explicit: the three days exist to reduce specific uncertainties, ranked by what each day can answer that nothing else can. The page must carry that reasoning. Same audience (Matt, forwarding to his manager), same tone: logistics with reasons, a draft that invites correction.

## The five content changes

All replacement copy is provided verbatim in `kickoff_page_v3_copy.md`. Do not paraphrase it; the wording is deliberate. Locations reference the current build's Kickoff surface.

1. **Header subline.** Replace the current subline ("...This page is logistics with reasons...") with copy block 1. The change: the three days are framed as spent where they reduce the most uncertainty.

2. **New strip: "What the three days are for."** Insert between the section 01 heading row and the "Before we arrive" checklist: a three-item horizontal strip (numbered 1-3, same typographic grammar as the ground-rules strip in section 02). Copy block 2. These are the three questions the workshop exists to answer; visually quieter than the day cards, they set up why the days are shaped as they are.

3. **Day 3 card, morning block.** Replace the Day 3 morning heading and items with copy block 3 (heading "Morning: measures from decisions, then the twelve" plus three items), and replace the Day 3 output line with the updated one in the same block. The substance: the room hypothesizes measures from the decisions BEFORE the existing candidate list is opened, and decisions left underserved get flagged.

4. **Trace card honesty line.** Append one sentence to the body of snapshot card 08 (the 20-project trace sample), copy block 4.

5. **Section 03 intro line.** Replace the frame line above the decisions grid with copy block 5 (adds the reverse direction: a decision no measure serves tells us what the candidate list still owes).

## Footer

Bump the version strip from "v2 · July 2026" to "v3 · August 2026". Add a v2 archive link alongside the existing v1 link, following the same pattern ("Earlier versions: v1 · v2"). If a static v2 snapshot file needs to exist for that link, generate it from the current build before applying changes (same approach as the existing v1 file).

## Hard rules (unchanged from the original Kickoff prompt)

- No pricing anywhere.
- No em-dashes.
- No names except Matt and Eric. The command center developer appears as "the PBI developer" / "the command center team."
- No DHW-internal vocabulary. Specifically for this update: no "priors," no "uncertainty model," no "information value," no gate codes, no "Hubbard." The provided copy already respects this; keep it that way.
- No probabilities or numeric ranges anywhere on the page (the "3 in 10 or 7 in 10" phrasing in copy block 2 is illustrative speech, not a claimed estimate; keep it exactly as written).
- The decision inventory stays visually DRAFT.
- Existing pages, reactions, and URLs untouched; Listen-page reaction state must survive.

## Post-build verification checklist

1. grep built page for $ amounts, "fee", "rate", em-dashes: expect zero.
2. Header subline updated; the three-item "what the days are for" strip present above "Before we arrive."
3. Day 3 morning shows decisions-first then the twelve; Day 3 output line updated.
4. Trace card (08) ends with the honesty sentence.
5. Section 03 frame line carries the reverse-direction sentence.
6. Footer reads v3 · August 2026 with working v1 and v2 archive links.
7. Days 1 and 2 cards, snapshot cards 01-07, ground rules, decisions grid, section 04: byte-identical to current.
8. Confirm all other surfaces unchanged and reactions persist.

## Files provided with this prompt

- kickoff_page_v3_copy.md (the five copy blocks, verbatim)
- 22_kickoff_run_of_show.md (updated run-of-show; source of truth for the Day 3 change)
- Existing site source (current build)
