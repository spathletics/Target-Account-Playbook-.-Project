# The launch window is the buying window

A launch-window account playbook built by Sasha Podgurskyy as a work sample for the Quantified Business Development Representative role.

It tracks 13 life sciences accounts by their FDA trigger: a recent approval, or a decision coming up. Each account has the buyers to reach, a Sales Navigator search to find them and the pain to test. Accounts in active pursuit also have a first-touch email and a call opener, and the Tier 1 ones have a five-touch sequence.

**Live page:** add the GitHub Pages link here once Pages is turned on.

## What's on the page

- **Launch radar:** every account plotted by days since approval or days until the FDA decision, with the outreach windows marked.
- **This week:** next steps due in the next seven days, plus anything that needs attention. Examples are a watchlist account inside six weeks of its decision, a decision date that has passed, or an overdue follow-up.
- **Pipeline:** Watchlist → Researching → Contacted → Engaged → Meeting booked → Handed off. Open any account to see the full brief, move its stage, log an update or edit it.
- **Export CSV** for the current view.

Changes a visitor makes stay in their own browser. **Reset to original** brings back the published version.

## Editing the accounts

Everything lives in `index.html`. The account data is the JSON block near the bottom, in `<script type="application/json" id="seed">`.

1. Edit the account in that block.
2. Change `"version"` at the top of the block. Returning visitors then get the new data instead of their old copy.
3. Update `nextDate` values before sharing the link. Next steps that are past due show as "needs attention".

## Publishing

1. In the repo settings, open **Pages**, choose **Deploy from a branch** and pick `main` with the root folder.
2. If you rename the repo, also update the `og:image` URL in the `<head>` of `index.html`. Link previews in LinkedIn, Slack and email need the full URL of `og-image.png`.
