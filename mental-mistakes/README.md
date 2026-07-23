# Mental Mistakes — Lead Magnet Funnel Pages

Static pages for Diandra Asbaty's free lead magnet, **"All the Mental Mistakes
I've Made (So You Don't Have To)"** — a guide for bowling parents.

**Source of truth:** Google Doc *"Mental Mistakes Funnel — Emails + Full Setup
(FINAL v2)"* (supersedes the earlier "Nurture Emails + GHL Setup" doc). The email
nurture sequence and the full GHL setup live there; these files are the web assets.

## Files

| File | Serves at | Purpose |
|---|---|---|
| `index.html` | `/mental-mistakes` | Opt-in landing page. Two form slots. |
| `thank-you.html` | `/mental-mistakes/thank-you` | Redirect target after opt-in. Two offers. |
| `../mental-mistakes-homepage-embeds.html` | (not published) | Placement demo + 3 copy-paste homepage snippets. |

## Developer TODO (before go-live)

These are the only placeholders left in the HTML — search for `DEVELOPER` and the
`#GHL_` markers:

1. **Opt-in forms** — replace the two placeholder forms in `index.html` (marked
   `GHL FORM EMBED #1/#2`) with the GHL form (First Name + Email).
   Tag on submit: `mental-mistakes-lead`. Set the GHL form redirect to
   `/mental-mistakes/thank-you`.
2. **Homepage forms** — same GHL embed in the two snippets in
   `mental-mistakes-homepage-embeds.html` (guide section + footer block).
3. **Thank-you offers** in `thank-you.html`:
   - `#GHL_CHECKOUT_URL` → Junior Gold Debrief $24.97 checkout.
   - `#GHL_MINDSET_RESET_TRIAL_URL` → Mindset Reset free-first-month trial offer.
4. **Guide PDF** — host `all-the-mental-mistakes.pdf` in GHL Media Storage; use its
   URL in Email 1's download button.
5. **Homepage placement** — paste the three snippets from
   `mental-mistakes-homepage-embeds.html` (announcement bar site-wide, guide section
   below the hero, footer block replacing the current newsletter signup).

The placeholder forms currently `GET` to the thank-you page so the flow is
click-testable before the GHL embeds go in.
