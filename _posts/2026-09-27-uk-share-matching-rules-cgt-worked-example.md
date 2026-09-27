---
layout: post
title: "UK Share Matching Rules for Capital Gains Tax: Same-Day, 30-Day and Section 104, with a Worked Example"
description: "How HMRC matches a share sale: same-day rule, the 30-day 'bed and breakfast' rule, then the Section 104 pool. One fully worked example with dealing costs, a buy-back within 30 days and the gain calculated to the penny."
date: 2026-09-27
last_modified_at: 2026-09-27
categories: [uk-tax, investing]
tags: [capital gains tax, section 104, share matching, bed and breakfast rule, HS284]
---

If you've bought the same shares more than once and then sold some, you can't just take "the average price I paid" and subtract it from what you sold for. HMRC has a fixed order for deciding **which** shares you sold, and that order can change your gain by hundreds of pounds. This guide explains the three matching rules and then works through one example, step by step, to the penny.

*Rules and figures checked against HMRC and GOV.UK pages on 27 September 2026 (sources at the end).*

## Who this applies to

These rules are for individuals disposing of **shares of the same class in the same company** (units in unit trusts, investment trust shares and OEIC shares are treated the same way, per HMRC helpsheet HS284). They don't apply to everything:

- **ISAs:** GOV.UK lists "any shares that are not in an ISA or PEP" as chargeable, and gains from ISAs or PEPs are among the things you don't pay Capital Gains Tax on. Shares inside an ISA are outside CGT.
- **SIPPs and other registered pension schemes:** HMRC's Capital Gains Manual (CG67650) says "The disposal of an investment held for the purposes of a registered pension scheme is not a chargeable gain." Investments held in your SIPP are outside CGT.
- Share reorganisations (splits, rights issues, takeovers), employee share schemes, EIS and VCT shares have extra rules not covered here (see HS284 and HS285).

## The matching order

HMRC helpsheet HS284 (section 2) and the Capital Gains Manual (CG51555) set out the order. When you sell, the shares you sold are matched:

1. **First, with shares bought on the same day** (the "same day" rule).
2. **Second, with shares bought in the 30 days after the sale** (the "bed and breakfasting" rule), provided you were UK resident when you bought them.
3. **Third, with shares in your Section 104 holding** (the pool).

If those three don't cover the whole sale, the rest is matched with later purchases, earliest first. That only happens in unusual cases, like selling shares you don't yet hold.

One more rule matters a lot: **shares matched under rules 1 and 2 never enter the pool** (CG51555, note on TCGA92/S105(3) and S106A(5ZA)).

### Rule 1: the same-day rule

From CG51560: all shares of the same class bought on the same day are treated as **one** acquisition, and all sold on the same day as **one** disposal. If you buy and sell on the same day, the sale is matched first against that day's purchases. If you bought more than you sold that day, the surplus goes into the pool (unless it's needed for a 30-day match). If you sold more than you bought, the excess is matched in the normal way.

### Rule 2: the 30-day ("bed and breakfast") rule

A sale is matched with shares of the same class that you acquire **within the 30 days after** the sale (CG51560). This stops people selling to crystallise a gain or loss and buying straight back. HMRC's own examples show where the line falls:

- Sold 1 July 2011, bought back 31 July 2011: that's 30 days later, so it **is** matched (CG51560 Example 1).
- Sold 28 February 2009, bought 31 March 2009: that's 31 days later, so it is **not** matched, and the sale comes out of the pool instead (CG51560 Example 3).

The gain on a 30-day match is simply the (apportioned) net sale proceeds minus what you paid for the shares you bought back (HS284 section 3).

### Rule 3: the Section 104 pool

Everything else goes into one pool per share line: a running total of **number of shares** and **allowable cost**. The allowable cost includes the price paid **and** the costs of buying, such as dealing fees (CG51575). GOV.UK also lists Stamp Duty Reserve Tax paid when you bought as a deductible cost.

When you sell part of the pool, the cost you take out is:

> **pool cost × (shares sold ÷ shares in the pool)**

(HS284 section 4. CG51575 notes that in strict terms the part-disposal formula uses market values, but in practice HMRC accepts apportionment by number of shares.) The pool then shrinks by those shares and that cost.

Selling costs (your dealing fee on the sale) reduce the proceeds. HMRC's examples in CG51590 state that "Figures for disposal proceeds are net of incidental costs of disposal."

## A fully worked example

One holding, ABC plc ordinary shares, bought and sold through a UK dealing account (not an ISA). Every trade has a **£10.00 dealing fee**. To keep the arithmetic clear, there's no stamp duty in the example; if you paid SDRT, add it to that purchase's cost.

| # | Date | Trade | Shares | Price | Money |
|---|---|---|---|---|---|
| B1 | 10 May 2026 | Buy | 1,000 | £4.00 | £4,000 + £10 fee = **£4,010.00** cost |
| B2 | 12 Aug 2026 | Buy | 500 | £4.60 | £2,300 + £10 fee = **£2,310.00** cost |
| B3 | 3 Nov 2026 | Buy | 200 | £5.00 | £1,000 + £10 fee = **£1,010.00** cost |
| S1 | 3 Nov 2026 | Sell | 800 | £5.10 | £4,080 − £10 fee = **£4,070.00** net proceeds |
| B4 | 20 Nov 2026 | Buy | 300 | £4.80 | £1,440 + £10 fee = **£1,450.00** cost |
| B5 | 5 Dec 2026 | Buy | 400 | £4.90 | £1,960 + £10 fee = **£1,970.00** cost |
| S2 | 10 Feb 2027 | Sell | 600 | £5.20 | £3,120 − £10 fee = **£3,110.00** net proceeds |

There are no other trades in ABC plc, and none in the 30 days after 10 February 2027. The investor is UK resident throughout.

### Step 1: build the pool up to the first sale

| | Shares | Pool cost |
|---|---|---|
| B1 | 1,000 | £4,010.00 |
| B2 | + 500 | + £2,310.00 |
| **Pool before 3 Nov** | **1,500** | **£6,320.00** |

B3 is bought on the same day as the sale, so it isn't added to the pool yet: rule 1 gets first claim on it.

### Step 2: match the sale of 800 shares on 3 November 2026

Net proceeds are £4,070.00 for 800 shares, which is **£5.0875 per share**. Each block of shares matched gets its share of the proceeds.

**Rule 1, same day: 200 shares matched with B3**

- Proceeds: 200 × £5.0875 = £1,017.50
- Cost: £1,010.00
- Gain: **£7.50**

**Rule 2, next 30 days: 300 shares matched with B4 (20 November, 17 days later)**

- Proceeds: 300 × £5.0875 = £1,526.25
- Cost: £1,450.00
- Gain: **£76.25**

B5 (5 December) is 32 days after the sale. The 30-day window ends on 3 December, so B5 is **not** matched and will go into the pool.

**Rule 3, pool: the remaining 300 shares**

- Cost: £6,320.00 × 300 ÷ 1,500 = £1,264.00
- Proceeds: 300 × £5.0875 = £1,526.25
- Gain: **£262.25**

**Total gain on the 3 November sale: £7.50 + £76.25 + £262.25 = £346.00**

Check: £4,070.00 proceeds − (£1,010.00 + £1,450.00 + £1,264.00 = £3,724.00) = **£346.00** ✔

Pool after the sale: 1,500 − 300 = **1,200 shares**, £6,320.00 − £1,264.00 = **£5,056.00**. B3 and B4 never enter the pool, because they were used by rules 1 and 2.

### Step 3: add B5 to the pool

| | Shares | Pool cost |
|---|---|---|
| After S1 | 1,200 | £5,056.00 |
| B5 (5 Dec 2026) | + 400 | + £1,970.00 |
| **Pool** | **1,600** | **£7,026.00** |

### Step 4: the sale of 600 shares on 10 February 2027

No same-day purchase and no purchase in the next 30 days, so all 600 come from the pool.

- Cost: £7,026.00 × 600 ÷ 1,600 = **£2,634.75**
- Gain: £3,110.00 − £2,634.75 = **£475.25**

Pool left: **1,000 shares** costing £7,026.00 − £2,634.75 = **£4,391.25**.

### Step 5: the tax-year total

Both sales fall in the 2026 to 2027 tax year (6 April 2026 to 5 April 2027):

**£346.00 + £475.25 = £821.25 total gains**

### What if you'd just used an average price?

If you ignored rules 1 and 2 and took the 800 shares sold on 3 November out of the pool at average cost (£6,320.00 × 800 ÷ 1,500 = £3,370.67), you'd report a gain of £4,070.00 − £3,370.67 = **£699.33** instead of **£346.00**, and your pool would be wrong for every later sale too.

### The same maths in pence (second check)

Working in whole pence avoids rounding surprises:

- Net proceeds 408,000p − 1,000p = 407,000p; ÷ 800 = 508.75p a share, so 50,875p per 100 shares.
- Same day: 2 × 50,875 − 101,000 = **750p**
- 30 days: 3 × 50,875 − 145,000 = **7,625p**
- Pool: 632,000 × 300 ÷ 1,500 = 126,400p cost (this divides exactly); 3 × 50,875 − 126,400 = **26,225p**
- Total: 750 + 7,625 + 26,225 = **34,600p = £346.00** ✔
- Pool after S1: 632,000 − 126,400 = 505,600p; plus B5 197,000p = 702,600p
- S2 cost: 702,600 × 600 ÷ 1,600 = 263,475p; gain 311,000 − 263,475 = **47,525p = £475.25** ✔

## Allowance and rates for 2026 to 2027

- **Annual exempt amount (tax-free allowance): £3,000** for 2026 to 2027, the same as 2024 to 2025 and 2025 to 2026 (GOV.UK). You only pay CGT on total gains above it, after losses. In the example, £821.25 is below £3,000, so there's no CGT to pay.
- **Rates on gains from 6 April 2026:** 18% on the part that falls within the basic rate band and 24% above it (GOV.UK, "Capital Gains Tax rates").
- **Reporting even below the allowance:** GOV.UK says that if you're registered for Self Assessment, you need to report your gains on your tax return if the total amount you sold assets for was more than **£50,000** (for 2023 to 2024 onwards). The example's sales total £7,200.00, well below that.
- **When:** the tax year runs from 6 April to 5 April. Online Self Assessment returns are due by 31 January after the tax year ends; for 2025 to 2026, that's 11:59pm on 31 January 2027 (GOV.UK).

## Common mistakes

1. **Using a simple average of every purchase.** Same-day and 30-day purchases are taken out first, and they never join the pool.
2. **Forgetting the buy-back.** If you sell and buy back within 30 days, the sale is matched with the new shares (up to the number bought back), not the old ones, so the gain or loss you expected can shrink or disappear.
3. **Miscounting 30 days.** The window is the 30 days after the sale. HMRC's example treats a purchase 30 days later as matched and one 31 days later as not.
4. **Leaving out costs.** Buying costs (dealing fees, SDRT) go into the cost; selling costs reduce the proceeds.
5. **Mixing accounts.** Shares in an ISA or SIPP are outside CGT. Outside those wrappers, the matching rules apply to all your shares of the same class in the same company held in the same capacity (CG51555), so shares of the same company held with two brokers are normally one pool, not two.
6. **Not keeping the pool running.** Each sale's cost depends on the pool left by earlier sales, so a mistake carries forward.

## A free record book for one holding

If you'd rather not do this by hand for every trade, I made a free spreadsheet that applies these matching rules for one holding. It shows how each sale was matched, the allowable cost, the gain or loss, the running pool and a tax-year summary. It's a record-keeping tool: it doesn't work out the tax you owe. [UK Share CGT Record Book (Lite), free](https://khalidmasscom.gumroad.com/l/wdatk?utm_source=blog&utm_medium=article&utm_campaign=p003_lite&utm_content=article_end) (Built for Excel; Google Sheets compatible).

## Sources (checked 27 September 2026)

- HMRC, HS284 Shares and Capital Gains Tax (2026): https://www.gov.uk/government/publications/shares-and-capital-gains-tax-hs284-self-assessment-helpsheet/hs284-shares-and-capital-gains-tax-2026
- HMRC Capital Gains Manual CG51555 (identification order): https://www.gov.uk/hmrc-internal-manuals/capital-gains-manual/cg51555
- CG51560 (same day and 30-day rules, with examples): https://www.gov.uk/hmrc-internal-manuals/capital-gains-manual/cg51560
- CG51575 (the Section 104 holding): https://www.gov.uk/hmrc-internal-manuals/capital-gains-manual/cg51575
- CG51590 (worked examples): https://www.gov.uk/hmrc-internal-manuals/capital-gains-manual/cg51590
- CG67650 (pension schemes): https://www.gov.uk/hmrc-internal-manuals/capital-gains-manual/cg67650
- GOV.UK, Capital Gains Tax allowances: https://www.gov.uk/capital-gains-tax/allowances and rates and allowances by year: https://www.gov.uk/government/publications/rates-and-allowances-capital-gains-tax/capital-gains-tax-rates-and-annual-tax-free-allowances
- GOV.UK, Capital Gains Tax rates: https://www.gov.uk/capital-gains-tax/rates
- GOV.UK, what you pay CGT on (ISAs): https://www.gov.uk/capital-gains-tax/what-you-pay-it-on
- GOV.UK, work out your gain on shares (deductible costs): https://www.gov.uk/tax-sell-shares/work-out-your-gain
- GOV.UK, work out if you need to pay (the £50,000 reporting rule): https://www.gov.uk/capital-gains-tax/work-out-need-to-pay
- GOV.UK, Self Assessment deadlines: https://www.gov.uk/self-assessment-tax-returns/deadlines

*This article is educational, and the record book is a record-keeping tool. Neither is tax or financial advice. Rules and allowances change, so check HMRC's current guidance, or ask a qualified adviser, before you file.*