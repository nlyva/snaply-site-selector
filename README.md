# snaply-site-selector
Interactive photo booth location and price simulator for Snaply: break-even, payback, 4 AZN vs 8 AZN
# Snaply Site Selector

Interactive simulator for a self-service photo booth business in Baku. It answers two questions: where should Snaply place its first booth, and what price keeps the business sustainable at each location?

**Live demo:** https://nlyva.github.io/snaply-site-selector/

## What it does
Choose a mall, then change the session price, rent and daily sessions. The tool shows monthly result per booth, break-even sessions per day and payback in months. A chart compares the 4 AZN survey price with the 8 AZN base price.

## Context
Built from the Snaply business plan proposal, a group project for Business Policy & Strategy - Capstone I (BUSA-4790) at ADA University. Group members: Nazrin Aliyeva, Nigar Abdullayeva, Mohadeseh Sadat Mousavi Maleki, Nargiz Aghamaliyeva, Farah Amrahova. My contribution: [describe your part, e.g. financial model, supplier comparison, this simulator].

## Method
- Contribution per session = (price + add-on revenue per session) x (1 - payment fee) - media cost
- Break-even sessions per day = (fixed costs + rent + depreciation) / (contribution per session x 30 days)
- Payback = funding requirement per booth / monthly operating surplus before depreciation
- Inputs come from the proposal's cost model: media 1.20 AZN per session, 3% payment fees, 600 AZN monthly add-on revenue per 1,800 sessions, 16,652 AZN funding per booth

## Key finding
Price is the deciding assumption. At 340 AZN rent, a booth needs about 13 sessions per day to break even at 4 AZN, but about 6 at 8 AZN.

## Limitations
- Sessions per day is an input, not a measured result. The main survey and mall footfall counts are still pending, and the only footfall figure (Deniz Mall) is an unofficial estimate.
- The pilot survey had 37 ADA students, so the 3-4 AZN willingness to pay is not representative of Baku mall visitors.
- Rents are listing benchmarks, not written mall quotes. Marketing costs are excluded.

## Next steps
Replace the sessions input with a demand curve from the Gabor-Granger survey, add a Monte Carlo break-even probability, and build a Streamlit version.
