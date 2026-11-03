# BRAND-001 validation

## Setup

Repository: `git@github.com:bvd6-ui/Brand-Studio.git`. Node v24.21.0, npm 12.2.0. README and both npm manifests tracked in origin/main. `npm ci` succeeded after sandbox DNS restrictions required an authorized retry. npm reported seven moderate dependency advisories; no forced dependency changes applied.

First baseline attempt: formatting/lint passed; sandbox prevented server tests. Authorized rerun passed seven server tests; browser tests could not launch because Chromium was absent. `npm run setup:browser` installed the configured Chromium successfully.

Baseline rerun: `npm run check` passed formatting, lint, seven server tests and ten Chromium browser tests before source edits.

## Implementation

- Initial branded run identified duplicate CSS selectors and formatting; these were fixed in source without relaxing rules. The next `npm run check` passed all seven server and ten browser tests.
- Expanded existing integrity/axe and narrow-overflow checks to cover all three new exploration routes. The first expanded run had 15 passes and one studio axe timeout during concurrent visual review.
- Final `CI=1 npm run check`: **passed** formatting, HTML/CSS/JS lint, **7 server tests and 16 Chromium browser tests** (27.1s browser phase). CI mode uses the repository’s existing two-worker configuration. All 16 passed on their first attempt in this run. No rules or assertions were weakened.
- AI inspected actual storefront, style guide, studio and both hero studies at desktop (1280px) and narrow (375px) widths. No clipped content observed; one-color logo remained readable at its actual 175px desktop and 150px narrow navigation sizes. Guide and storefront share actual logo assets, color roles and type families. Desktop screenshot capture once timed out during concurrent browser testing; later capture succeeded.
- Browser DOM inspection confirmed both studies have identical headline, support, product facts, image source and action destination; both product images loaded. Modernist computed font is the system sans-serif stack; postmodernist is Georgia/Times serif. Both study actions reached the working storefront size form.
- Museum artwork references were visually inspected at the original MoMA and SFMOMA pages; no reference images copied into the repository.
- Reviewed diff and product claims: demo price clearly fictional, product specifications unspecified, no fabricated testimonials/urgency or enrollment. Existing `shop.js` is unchanged. Tests cover keyboard size selection and bag action, reset, live reload, local links, image loading, runtime errors and selected axe rules. Passing axe is not proof of complete accessibility.

### One actual test for discussion

In `tests/browser/studio.spec.js`, the negative case opens the storefront with no selected size and clicks **Add to demo bag**. Assertions: the size error is visible and nonempty; the bag count remains **0**. Result: **passed** in the final run. Learner interpretation is pending; do not treat the automated result as their explanation.

## Human evidence

Only the earlier neutral-storefront bag observation is available. Branded-page impression, keyboard and narrow-view observations, test interpretation, record review, and keep/merge decision remain pending.
