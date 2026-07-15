# The Scoreboard Question · handoff notes

Files: `The Scoreboard Question.dc.html` (the site), `The Research File.dc.html` (print-clean research page, linked only from the case-room foot), `uploads/scoreboard_site_structure_and_copy_v4.md` (the copy as shipped).

## 1 · The copy revision (supersedes "copy is final")

Per DHW direction mid-build, the v3 copy was re-edited against THE-TELL before shipping: em dashes removed, throat clearing cut, reframe-by-negation removed, and all sales-denial framing dropped ("Two essays, not a proposal," "What this site is not," "nothing here books a meeting," "No proposal, on purpose," "Nothing on this site asks you to buy back a problem"). Facts, structure, and every verbatim Matt quote are unchanged. The full revised copy is in the v4 file, diffable against v3. Key replacements:

- H1: "Two essays, not a proposal." → "Two essays, written for you."
- "What this site is not" block → "Yours to keep" (positive form of the same two commitments).
- Close block 3 now opens on "Two things stand exactly as said on the call."

## 2 · Decisions owed by a human

- **The essays still carry em dashes.** They ship verbatim from `article_03_recut.md` / `article_04_piece_two_draft.md` (recently hand-edited files, marked "content ships as-is" in v3). If THE-TELL should apply to them too, say so and they get the same pass with meaning preserved.
- **The research file still carries em dashes.** Build note 5 allowed mechanical edits only ("change nothing else"), so only those were made: all `citeturn…` markers stripped; the two "the user's" phrasings (deep dives · MDIC pilot inference; cross-cutting · third paragraph) now read "a sustaining-portfolio leader's."
- **Build note 6, pending domain-set edit:** the report's Transfer section names the fourth domain "Execution and Learning"; Essay II and the executive summary use "Quality-system health" / "Quality-System Effectiveness." Left as written per instructions. The report also says "the Microsoft estate" (Transfer, final paragraph) — reads as an artifact of the source draft; left as written.
- **Engage walkthrough:** the v3 sentence promised "thinking from two of our people," but Block 2 ships hidden. The clause is dropped from the walkthrough; restore it when the block ships in v2. Block 2's placeholder is preserved as a source comment in the Close section.

## 3 · Spec ambiguities resolved

- **Visual system:** the brief described the reference as "dark ground, IBM Plex, teal/ember/gold/violet." The actual reference site (in this project) and the bound Editorial Signal system are paper `#F2F0EB`, Inter / Instrument Serif / JetBrains Mono, signal red `#D64A1F`. Followed the reference as observed.
- **"Send to Dark Horse Works":** no DHW email address exists in the provided materials, so no mailto was invented. The record compiles on the Close surface and exports as `scoreboard-record.txt` (plain-text download, per the brief's allowance). If a mailto is preferred, supply the address.
- **Back links:** case room "← Back to the essays" goes to the Bridge; the research page's "← Back to the case room" returns to the site with the case room open.
- **Case-room foot links:** "Read online" opens the research page; "download print version" opens it with the print dialog.

## 4 · Invented strings (everything not in v3/v4 copy)

Nav: "Case room" · lock kickers "Listen · the second lock" through "Close · the sixth lock" (reference grammar; Engage uses the spec kicker) · Listen legend "Relayed · Matt's words / Our read · inferred" (from the spec's own parentheticals) · card controls "This lands / Affirmed," "Not quite / Edited," "Skip / Skipped," "More context / Less," "Previous," "Next point," "Go to the bridge," "Save correction," "Cancel," input placeholder "Add a point we did not capture," "Add card," added-card headline "Added by Matt," tag "Added," correction note "Your correction · on the record" · bridge buttons "Read Essay I / Read Essay II" · essay flag control "too close to home? / flagged," essay foot "Continue to Essay II," "Continue to the close" · record block "The record," its caption, empty state "Nothing on the record yet.," "Download the record" · case flag "Flag / Flagged" · footer "Reset session" + confirm text · research page: title "The research file · Dark Horse Works," kicker "The research file," "← Back to the case room," "Print / save as PDF."

## 5 · Mechanics

- State (affirmations, corrections, additions, expansions, essay flags, case flags, current surface) persists in `localStorage`; "Reset session" clears it.
- Keyboard 1–6 jumps locks; `#cases` in the URL opens the case room.
- `noindex, nofollow` meta and the page title mount at runtime on both pages; the client's name appears only in the on-page Engage kicker, never in titles, slugs, or metadata.
- Print: essay surfaces and the research page print clean (chrome, flags, and buttons hidden; white ground; letter size).
- No analytics, no trackers, no third-party embeds; fonts load from Google Fonts only.
