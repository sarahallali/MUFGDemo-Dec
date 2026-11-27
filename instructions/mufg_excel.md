# MUFG Excel Copilot Demo – Uncover New Data Insights

> Everything in this demo is fictional – FICTIONAL – FOR TRAINING USE ONLY. No MUFG or client data is used.

**Scenario:** You're **Priya Raman**, Portfolio Manager at MUFG EMEA. It's **Wednesday 21 October 2026**. Before next week's credit review, Haruka (Head of Corporate Banking) needs two answers:

1. How did the EMEA corporate loan book perform in Q3 2026?
2. How do the three options for the €800m Fabrikam loan – keeping **€200m, €250m or €300m** – compare with the bank's limits?

**Timing (60 minutes):** opening and story so far 7 · Part 1 11 · Part 2 15 · Part 3 12 · five-minute challenge 7 · wrap-up 8

## Story so far (30 seconds)

Fabrikam Industries, a long-standing client in Tokyo, wants to buy Contoso Energy Materials, a European battery-recycling company, and asks MUFG EMEA to lead an €800m loan. The Corporate Banking team has six weeks to check the deal and propose how much of the loan the bank keeps: €200m, €250m or €300m. Today's chapter: week 3, the numbers.

## Demo setup

**Use:**

- [Meridian_Portfolio_Q3_2026.xlsx](../files/Meridian_Portfolio_Q3_2026.xlsx) – 150 fictional loans, the quarterly trend, sector limits and the deal pipeline
- [Meridian_Fabrikam_Analysis.xlsx](../files/Meridian_Fabrikam_Analysis.xlsx) – the deal figures and the three hold options

> **NOTE:** Copilot in Excel works on files saved in OneDrive with AutoSave on. The data is already formatted as Excel tables. Keep a clean copy of the portfolio workbook: Part 1 fixes its data errors, so reset it before each session.

**What's in the portfolio workbook:** `Portfolio_Exposures` (the loans) · `Quarterly_Trend` (last eight quarters) · `Risk_Appetite_Limits` (sector limits) · `Pipeline` (upcoming deals) · `Data_Dictionary` · `About`

## Part 1 – Understand and clean the data

**1. Get the big picture**

**Where:** Copilot in Excel – any worksheet

```text
Summarise what this workbook contains and what each sheet could be used for in a portfolio review.
```

**Look for:** one line per sheet, including the limits and the pipeline.

**Say:** Start every new workbook by asking what's in it.

**2. Explain the columns**

**Where:** Worksheet `Portfolio_Exposures`

```text
Explain the columns in the Portfolio_Exposures table in plain language for someone new to credit portfolios.
```

**Look for:** commitment versus drawn, rating grade, IFRS 9 stage, RWA.

**Say:** Plain-language explanations help new joiners read the data correctly.

**3. Check the data before you trust it** (one prompt at a time)

**Where:** Worksheet `Portfolio_Exposures`

```text
Highlight any rows where the Facility_ID appears more than once.
```

```text
Highlight rows where Drawn_EURm is greater than Commitment_EURm.
```

```text
Show the distinct values in the Country column and how many rows use each one.
```

```text
Which rows have a blank Rating_Grade?
```

**Look for:** the four problems in the [appendix](#appendix-data-errors-built-in-on-purpose). Fix them live: delete the second copy of MER-0123 (row 125); change MER-0122's drawn amount from 63 to **36** ("the data owner confirmed it"); change "NL" and "The Netherlands" to **Netherlands**; **leave the two blank ratings blank** and flag them to Credit Risk. The Industrials share on `Risk_Appetite_Limits` moves from 13.54% to **13.61%** once the duplicate is gone.

**Say:** Copilot finds the problems; people decide the fix. Never let AI guess a credit rating.

## Part 2 – Explore performance

**4. Add a calculated column**

**Where:** Worksheet `Portfolio_Exposures`

```text
Add a column called Utilisation_pct that divides Drawn_EURm by Commitment_EURm.
```

**Look for:** overall, about **69.9%** of the money promised has been drawn (€19,281m of €27,600m).

**Say:** Describe the calculation in words; Copilot writes the formula.

**5. Add the return**

```text
Add a column called RoRWA_pct that divides Annualised_Revenue_EURm by RWA_EURm.
```

**Look for:** overall **1.89%** – below the 2.5% hurdle for new loans. Infrastructure is highest (2.16%), Automotive lowest (1.66%).

**Say:** Check one row by hand before you trust a new column.

**6. Summarise by sector**

```text
Create a PivotTable showing total Commitment_EURm and RWA_EURm by Sector, sorted from largest to smallest,
with each sector's share of total commitments.
```

**Look for:** Energy & Utilities 14.0%, Industrials 13.6%, Infrastructure 11.7% …

**Say:** A PivotTable in one sentence – then you decide which view the committee needs.

**7. Compare with the limits**

```text
Compare each sector's share of commitments with the limits on the Risk_Appetite_Limits sheet.
Which sectors are above their early-warning level?
```

**Look for:** only **Industrials** – 13.61% against an early warning of 13.5% and a limit of 15%.

**Say:** Copilot reads two sheets together, so the limits sit next to the numbers.

**8. Spot the loans that need attention**

```text
Highlight facilities that are on the watch list or in IFRS 9 Stage 2 or Stage 3.
```

**Look for:** 14 loans – 13 in Stage 2 and one in Stage 3 (Drevanta Automotive Components, €45m).

**Say:** Highlighting is a starting point for Credit Risk, not a judgement on the client.

**9. Find the downgrades**

```text
Which sectors had the most rating downgrades this quarter? Compare Rating_Grade with Prior_Quarter_Rating.
```

**Look for:** 17 loans downgraded – Automotive 7, Chemicals & Materials 6. The two blank ratings are missing, not downgraded.

**Say:** Missing is not the same as downgraded. Check how Copilot treated the blanks.

**10. Chart the trend**

**Where:** Worksheet `Quarterly_Trend`

```text
Create a line chart of Industrials_Share_pct over the last eight quarters and describe the trend.
```

**Look for:** from 12.0% (Q4 2024) to 13.61% (Q3 2026) – up about 0.23 points every quarter.

**Say:** A chart plus a one-line description is ready for the review pack.

**11. What stands out?** (optional)

```text
What are the main trends in revenue, impairment charges and Stage 2 exposure over the last eight quarters?
What stands out in Q3 2026?
```

**Look for:** revenue up only 0.5% while lending grew 1.3%; impairment charges up to €15.4m from €7.0m; Stage 2 loans at €2,220m, 8.0% of the book.

**Say:** Ask what stands out, then check each point against the data.

## Part 3 – Compare the options

**12. Forecast**

**Where:** Worksheet `Quarterly_Trend`

```text
Forecast Industrials_Share_pct for the next four quarters based on the last eight quarters
and add the forecast to the chart. Explain the method you used.
```

**Look for:** a straight-line trend gives 13.86%, 14.10%, 14.33% and 14.56% (other methods may differ slightly). The share keeps rising even without the Fabrikam deal.

**Say:** Always ask for the method. A forecast is only as good as its assumptions.

**13. Compare the three options**

**Where:** Workbook `Meridian_Fabrikam_Analysis` · worksheet `Hold_Scenarios`

```text
For each hold option, explain the impact on Industrials concentration including the pipeline,
single-name limit usage and return on RWA. Which options stay within risk appetite?
```

**Look for:** see the [expected results](#appendix-expected-results-for-the-three-options) – €300m breaks the 15% limit.

**Say:** Copilot lays out the facts for each option; the credit review weighs them.

**14. Add a status column**

```text
Add a column that labels each option 'Within appetite', 'Early warning' or 'Breach' using the 15% limit
and the 13.5% early-warning level for Industrials concentration including the pipeline.
```

**Look for:** €200m and €250m – Early warning; €300m – Breach.

**Say:** Rules you give Copilot become formulas you can audit.

**15. Explain a formula before you rely on it**

```text
Explain the formula in the new status column step by step, and tell me what would change it.
```

**Look for:** the thresholds 15% and 13.5% referenced in the formula.

**Say:** Never share a number you can't explain.

## Five-minute challenge

Haruka: "I have five minutes before the credit review. What do I need to know?"

```text
Give me the three numbers Haruka needs before the credit review on the Fabrikam hold options, with the evidence for each.
Do not recommend an option.
```

**Look for:** 15.05% (€300m breaks the 15% limit) · 14.90% (€250m stays within it) · 3.20% return on RWA at €250m including other business, above the 2.5% hurdle.

**Say:** Copilot gathers the evidence; the credit review makes the call.

## Try it on your own work

```text
I work as a [role] in [department] at a bank in EMEA.
Suggest five ways I can use Copilot in Excel with the data I work with. For each: the business question,
a ready-to-use prompt, how my data should be structured, a suitable chart, and what I must validate before sharing.
Start simple, then add two advanced ideas. Ask me questions about my data first.
```

## Key takeaway

Copilot in Excel takes you from a raw extract to a clear comparison: clean the data, explore it in plain language, forecast and compare options – while you check every number and the people in the room make the decision.

## Appendix: data errors built in on purpose

Sheet `Portfolio_Exposures` (header in row 1):

| Issue | Row(s) | What you'll see | Fix |
|---|---|---|---|
| Duplicate loan | 98 and 125 | MER-0123 (Talara Media S.A., €130m) listed twice | Delete one copy |
| Drawn more than the limit | 124 | MER-0122 (Pelstra Foods B.V.): drawn 63, commitment 60 | Correct to 36 |
| Country written three ways | 6, 17, 28 | "NL", "NL", "The Netherlands" | Change to "Netherlands" |
| Missing ratings | 15 and 141 | MER-0014 and MER-0139 have no Rating_Grade | Leave blank; flag to Credit Risk |

Totals before the fixes: commitments €27,730m, Industrials 13.54%. After: **€27,600m**, Industrials **13.61%**.

## Appendix: expected results for the three options

| Final hold | Industrials share (incl. pipeline) | Status | Single-name limit used | Return on RWA (incl. other business) |
|---|---|---|---|---|
| €200m | 14.76% | Early warning | 78% | 3.03% |
| €250m | 14.90% | Early warning | 88% | 3.20% |
| €300m | 15.05% | Breach | 98% | 3.00% |

- The loan on its own earns 2.01% for every option – below the 2.5% hurdle. The hedging and cash-management business makes the difference.
- The largest hold that stays within the 15% limit, including the pipeline, is about **€282m**.
