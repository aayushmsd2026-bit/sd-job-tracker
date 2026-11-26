# Weekly update guide

This file tells the weekly update run how to refresh `jobs.json`. The page (`index.html`) only reads `jobs.json`, so the HTML does not change.

## Who the tracker is for

A Nepali professional based in Kathmandu with a full-time bank job:

- Data Analyst at a commercial bank in Nepal since July 2025: auto loan credit risk model (default prediction, automated approvals), credit card portfolio growth, HR analytics framework in Python.
- Senior Analyst at Daraz (Alibaba), 2023–2025: CRM and user incentives across Nepal, Bangladesh, Pakistan and Sri Lanka, with a US$1.1M monthly budget.
- Research Analyst at BBN / Business Brainz, 2021–2023: research for Fortune 500 clients in energy, banking and telecom (SWOT, PESTEL).
- Earlier: mortgage loan processing (Australian loans) and client servicing at an agency, including rural field research for a Gates Foundation project.
- MBA (Westcliff University); BBA (Kathmandu College of Management); Google certificates in Data Analytics and Project Management.
- Master's in Sustainable Development at Kathmandu University, started August 2026.
- About 6 years of total work experience. Uses Python. No SPSS or Stata listed.

Best-fit themes: green or climate finance, sustainable or SDG finance, financial inclusion, private sector development, green taxonomy or ESG in banking, and research, MEL or data roles in development work.

## What to include

- Roles in Nepal (mainly Kathmandu Valley) in sustainable development, climate, environment, green finance, financial inclusion, research, MEL or data.
- Remote or home-based roles that a Nepali national living in Nepal can actually apply for. UN home-based consultancies and internships usually qualify. Skip "remote" roles limited to the US, UK or EU.
- Skip roles that need a technical degree he does not have (engineering, medicine, forestry), roles needing 10+ years, and admin, driver, nursing or pure accounting roles.

## Sources to check every week

devjobsnepal.com · ain.org.np/vacancy · jobsnepal.com · merojob.com · manishsaru.com.np ·
icimod.org/get-involved/vacancies · careers.gggi.org · jobs.undp.org (Nepal and home-based) ·
jobs.unicef.org (location Nepal) · UN Women careers · impactpool.org · untalent.org (home-based finance and environment) ·
World Bank / IFC careers (Kathmandu) · iDE, Heifer, Practical Action, Helvetas, Swisscontact Nepal pages.

## Special watch

- ICIMOD Young ICIMOD Professionals Programme (YIPP). The last call was in July 2025 (deadline 31 July). It is not a fixed yearly call. Check ICIMOD's vacancies page every week, and closely from May to August. If a new call opens, add it as `open`, and put it first in the weekly message.

- Other entry programmes to check every week (add as `open` when a call is live):
  - ADB Young Professionals Program: opens early September, closes 30 September. Age 32 or under when joining. His best fit.
  - SANDEE research grant (ICIMOD): call usually opens late November, closes 31 December.
  - Asia Foundation Development Fellows: opens around November, closes early December.
  - World Bank Group YPP: opens 1 September, closes 30 September. Track it. Note the experience rule (2–6 years on the cut-off date). Count his professional experience from July 2021.
  - AIIB Graduate Program: usually opens December–January. Track it. Note the experience maximum for each stream.
  - UN YPP: only if Nepal is on that year's list of participating countries.
- `type` can also be "fellowship" (a grant, award or programme done alongside his job).

## Status rules

- `open`: a deadline on or after today was confirmed on the posting.
- `verify`: seen in the last 3 weeks, but no deadline found.
- `closed`: the deadline has passed. Keep strong-fit closed roles (fit 60+) for up to about 8 weeks as signals of roles that come back, then remove them. Remove other closed roles.
- Never invent a deadline, salary or requirement. If it is not on the posting, leave it out.

## Fit score (0–100)

- Theme fit, up to 40: green or climate finance, financial inclusion or SDG finance score highest; research, MEL or data in development next; general climate or environment lower.
- Skills fit, up to 30: data analysis, credit risk, banking, research, project management.
- Eligibility, up to 20: nationality allowed; experience asked is 6 years or less.
- Practicality, up to 10: Kathmandu or remote; can be combined with a full-time job (consultancy or part-time scores higher).

70+ = strong, 50–69 = good, below 50 = stretch. Write `why` in 2–3 short, plain sentences. Say what matches and what is missing.

## Pay (required for every role)

The person wants roles that pay more than his current job, or remote consultancies that add income on top of it. His salary is NOT stored anywhere. He enters it on the page, and it stays in his own browser. So every role needs a `type` and a `pay` estimate.

- `type`: "full-time", "consultancy" (part-time, remote or short-term; the page shows this as side income) or "internship".
- `pay`: `{ "min": NPR per month or null, "max": NPR per month or null, "basis": ..., "note": short plain text }`.
  - basis "posted": use the posting's own figure. Convert USD to NPR at the current rate, and annual pay to monthly.
  - basis "UN scale": work it out from the grade. Kathmandu minimums: NO-A about NPR 241,700/month; NO-B about NPR 294,900/month. NPSA-8 tracks NO-A and NPSA-9 tracks NO-B. G-grades and NPSA-1 to NPSA-7 are lower. Look up the current local scale if you can.
  - basis "market estimate": use the ranges in `pay_reference` in jobs.json (for example, INGO programme officer about NPR 80k–150k).
  - basis "unknown" or "stipend": leave min and max as null and explain in the note.
- Remove the full-time roles that pay clearly less (max below about NPR 90k/month) unless the fit is 75+. Keep consultancies; they are extra income.
- Update the `pay_reference` table if you find better 2026 data. Never invent a figure.

## jobs.json fields

`id` (unique slug), `title`, `org`, `location`, `mode` ("Nepal" or "Remote"), `deadline` ("YYYY-MM-DD" or null),
`status` ("open", "verify" or "closed"), `link` (the official posting or the page where it was found), `fit` (number),
`why`, `requirements` (short), `added` ("YYYY-MM-DD"), `type`, `pay` (see the Pay section). Set the top-level `updated` field to today's date.

## Privacy

The repository is public. Do not add the person's name, employer name, email or phone to any file.
