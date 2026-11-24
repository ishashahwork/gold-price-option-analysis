# Gold Price Returns and Option Analysis

A statistics coursework workbook exploring daily gold-price returns and a one-day European call option. The available work addresses the gold-price portion of a group assignment in Statistics for Data Science. The workbook uses 251 closing prices from 31 May 2022 to 26 May 2023 to calculate 250 daily log returns.

[Open the analysis workbook](gold.xlsx) · [View the workbook printout (PDF)](gold.pdf)

## Analysis and results

The workbook calculates log returns, standardizes them, and compares their empirical distribution with a normal distribution. It also tests a hypothesis about the return standard deviation, estimates the probability of exercising a call option, and applies a Black–Scholes formula to estimate its premium.

The saved workbook reports:

- A sample daily log-return standard deviation of approximately **0.00948**.
- A Kolmogorov–Smirnov statistic of **0.0641**, compared with the workbook's **0.0860** critical value at 5%.
- A one-sided variance-test p-value of **0.129** for the stated hypothesis that the population standard deviation is 0.01 versus less than 0.01.
- An estimated exercise probability of **40.2%** and option premium of approximately **$5.30** per troy ounce, under the workbook's assumptions, including a $1,944.10 starting price, $1,949.10 strike, 5.25% annual risk-free rate and one trading day to expiry.

These are the workbook's saved results, not independently validated conclusions. In particular, the normal mean and standard deviation are estimated from the same sample, so the usual one-sample KS critical value used in the workbook requires further review. Failure to reject normality does not prove the returns are normal. The sorted normalized values are stored as values rather than formulas, so changes to the price data require rebuilding that column before repeating the KS calculation. The accompanying explanation describes the risk-free rate as an assumption based on the US three-month Treasury yield in May 2023, but does not cite a source.

## Files and use

- [gold.xlsx](gold.xlsx) — the working analysis, data, formulas and saved results. Open it in Microsoft Excel or a compatible spreadsheet application; there is no code to install or run. Spreadsheet functions and recalculation may differ across applications.
- [gold.pdf](gold.pdf) — a 13-page printout of the workbook for viewing without spreadsheet software.
- [Problem 1 explanation](Statistics%20Group%20Assignment%20%28Problem%201%20Explanation%29.docx) — notes on the Black–Scholes inputs and premium calculation. The notes contain imprecise descriptions of the probability terms; consult a reliable reference before using them as a guide.

The original assignment brief and unrelated practice exercises remain in the local folder but are excluded from Git by `.gitignore`. The available folder does not contain a completed analysis of the assignment's separate Benford's Law problem, a complete written report, or standalone project images.

## Contribution and credits

This was a group assignment completed by Isha Shah, who carried out the analysis and created the workbook. The original source and redistribution rights for the historical price data are not documented in the available files.
