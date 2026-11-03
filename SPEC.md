# Brand Studio decisions

## Current stage

- Feature: **BRAND-001 — Unwritten storefront and live style guide**.
- Stage: Implementation checked and ready for learner review on `codex/brand-001-unwritten`; not kept or merged.
- Scope: two audience hypotheses, brief, two researched hero studies, original one-color SVG wordmark, coherent storefront/style guide, two ethical persuasion applications, existing size/demo-bag behavior.
- Learner authorized remaining design decisions to be made by AI. Those decisions below are recommendations implemented under that delegation, not learner explanations or completed human reviews.
- Workflow exception: GitHub issue creation was attempted before saving work, but the available browser is signed out. Local implementation continued under the learner’s explicit completion request. Sign-in is now resolved: [issue #1](https://github.com/bvd6-ui/Brand-Studio/issues/1).
- Next: learner reviews the short learning record and actual pages, discusses a test, then decides whether to keep/merge.

## Product boundary

Same plain white T-shirt illustration in both studies and storefront. Existing $28 USD is explicitly a fictional demo price. S/M/L/XL are demo sizes. Fit, fabric, manufacturing, shipping and sustainability are unspecified. No orders, payment, accounts, enrollment or persistent bag. No invented social proof or scarcity.

## Audience hypotheses

Both are assumptions, not validated research. Primary/secondary audiences were chosen or approved by the learner from AI suggestions; concerns and page needs below are AI elaborations.

| Tiny card               | Primary                                                   | Secondary                                                       |
| ----------------------- | --------------------------------------------------------- | --------------------------------------------------------------- |
| Situation               | Book lovers visiting bookstores or reading clubs          | Everyday shoppers choosing a plain shirt for casual wear        |
| Goal/meaning            | Thoughtfulness; space for their own ideas                 | Simple styling without needing a literary identity              |
| Concern (AI assumption) | A brand that dictates their identity or feels pretentious | Unclear product, size controls or misleading purchase claims    |
| Page should help decide | Whether the open-ended meaning feels like them            | Whether to try a clearly labeled white-shirt demo in their size |
| Evidence                | Learner choice; audience hypothesis                       | Learner approval; audience hypothesis                           |

## Early brand brief

| Decision                 | Agreement and provenance                                                                                       |
| ------------------------ | -------------------------------------------------------------------------------------------------------------- |
| Name                     | **Unwritten** — learner selected from three AI suggestions                                                     |
| Promise                  | **Space for your own ideas** — learner chose this meaning                                                      |
| Archetype                | **Sage** — requested by learner; brand character of curiosity and understanding, not a customer classification |
| Voice                    | **Curious, thoughtful, playful** — learner selected                                                            |
| Voice example            | “What will you write into today?” — associated AI example                                                      |
| Headline                 | **Leave room for your next idea.** — learner selected                                                          |
| Supporting line          | **The shirt is blank. What it means is up to you.** — AI selected under delegation                             |
| Learner predicted effect | Response retained only in the unreviewed local LEARNING.md; not published before accuracy review.              |

## Visual decision

[Compare both live studies](public/explorations/index.html). Both use the same headline, supporting sentence, white-shirt asset, fictional price and “Choose your size” action, linking to the working form.

| Item              | Implementation / provenance                                                                                                                                                                                                                                                                                                                                                                         |
| ----------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Modernist         | [Open margins](public/explorations/modernist.html): asymmetric grid, strong sans-serif hierarchy, restricted palette and rule. Reference: [Jan Tschichold, Die Frau ohne Namen, 1927, MoMA](https://www.moma.org/collection/works/5754). Full poster visually inspected in browser. Context: [MoMA, The New Typography](https://www.moma.org/calendar/exhibitions/1013).                            |
| Postmodernist     | [Notes in the margins](public/explorations/postmodernist.html): literary serif quotation, layered panels, broken outline and oversized quotation mark. Reference: [Wolfgang Weingart, Collage 9, 1975, SFMOMA](https://www.sfmoma.org/artwork/2014.753/). Artwork visually inspected in browser; used as an experimental precedent for layering, not labeled by the museum as this website’s style. |
| Applied direction | **Open margins**, AI choice under delegation. Clear space supports authorship and legible controls support the secondary audience. Restraint risks feeling impersonal. The alternative’s layering could support interpretation but distract from the product. Learner comparison/reason not yet evidenced.                                                                                          |
| SVG logo          | [Original path wordmark](public/assets/wordmark.svg): geometric UNWRITTEN lettering and a trailing blank line. One flat ink color, no font dependency, no grayscale simulation. No trademark clearance claimed.                                                                                                                                                                                     |
| Logo variants     | Same SVG at desktop navigation 175px, narrow navigation 150px, and enlarged/one-color views in [style guide](public/styleguide.html). Learner review pending.                                                                                                                                                                                                                                       |
| Shared identity   | [styles.css](public/styles.css): paper, ink, muted green, system sans-serif and monospace labels. Guide reads actual CSS color and spacing tokens via [styleguide.js](public/styleguide.js).                                                                                                                                                                                                        |

## Ethical persuasion

AI-selected applications under the learner’s delegation; learner explanation of an element’s benefit is not yet evidenced. These are design intentions, not proven conversion effects.

| Principle   | Actual interface/copy                                                                                     | Mechanism and visitor benefit                                                                                                                                         |
| ----------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Reciprocity | Free prompt: “What did the last page leave unsaid?” with a suggestion to write a question after a chapter | Offers useful reflection before asking for anything. No signup, purchase, or submitted response; can be used independently of the shirt.                              |
| Liking      | “Dog-eared pages. Open questions. Your kind of company.” and a welcome to readers at any stage            | Shared interests and a friendly voice can make the brand relatable. Welcomes the visitor without claiming existing members, testimonials, endorsements or popularity. |

## Evidence

| Spec ID   | Files                                                                                                                                           | Issue/PR                                                                         | Actual checks and observations                                                                                                                                        |
| --------- | ----------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BRAND-001 | [Storefront](public/index.html), [guide](public/styleguide.html), [studies](public/explorations/index.html), [logo](public/assets/wordmark.svg) | [Issue #1](https://github.com/bvd6-ui/Brand-Studio/issues/1); feature PR pending | See [validation](docs/brand-001-validation.md). Learner’s earlier baseline report is recorded locally; branded-page, keyboard and narrow-screen observations pending. |

## Keep requirements still pending

- Human review of applied direction/logo and an explanation of one useful page element.
- Learner interpretation of one actual test and personal branded-page, keyboard and narrow-view observations.
- Explicit accuracy/removal review of changed LEARNING.md before its excerpts are staged, committed or pushed.
- Issue and checked feature PR; learner keep/merge decision and verified merge.
- Publishing is separate, not requested or claimed. No optional next feature selected.
