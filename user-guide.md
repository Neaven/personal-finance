# Using Portfolio

A walkthrough of every page, sub-tab, and workflow. Screenshots are demo data (a fictional profile, "Alex Tan"), never real figures; image files live in `guide-screens/`.

Portfolio is a local-first personal-finance app built as a modular platform: stocks, dividends, options, funds, fixed income, property & mortgage, insurance, expenses, tax, estate, CPF, goals, net worth and a forward cash-flow projection, all feeding one dashboard. This guide walks every page and sub-tab in sidebar order, one screenshot at a time.

- **Where to start:** The Dashboard is the map: each tile links to the page it summarizes. Add your accounts first (Manage → Accounts), then the modules you use.
- **How it fits together:** Modules don't talk to each other directly. Each emits a cash flow, a balance-sheet line or a projected payment, and the Dashboard, Net Worth, Performance and Cash Flow pages aggregate whatever is registered.
- **Online version:** https://claude.ai/artifact/1ygGUTry963Yk4VQcHNuQP (private to the owner unless shared)

## Contents

- **Overview:** [Dashboard](#dashboard), [Net Worth](#net-worth)
- **Cash Flow:** [Cash Flow](#cash-flow), [Expenses](#expenses)
- **Investments:** [Stocks & ETFs](#stocks-etfs), [Dividends](#dividends), [Options](#options), [Funds](#funds), [Fixed Income](#fixed-income), [Performance](#performance)
- **Retirement:** [CPF](#cpf), [Goals](#goals)
- **Planning:** [Property](#property), [Insurance](#insurance), [Estate](#estate), [Tax](#tax)
- **Manage:** [Accounts](#accounts), [Profile](#profile), [Automations](#automations), [Settings](#settings)

---

# Overview

## Dashboard

The one-screen answer to “where do I stand.” Every tile is a live roll-up of a module below it, and each card header links to the page it summarizes.

![Dashboard](guide-screens/01-01-dashboard.png)

Headline tiles: net worth S$595,081 (assets S$951,975 less liabilities S$356,894), financial runway 10.2 years (liquid net worth ÷ yearly spend), emergency fund 41.5 months against a 6-month target, portfolio value S$127,960, lifetime return +19.99%, and CPF S$41,292 shown on its own because it isn’t spendable.

![Dashboard](guide-screens/01-02-dashboard.png)

Further down: the “What that’s made of” bar puts every asset and liability class on one scale, the Allocation donut re-cuts the portfolio by asset class, account, sector or position, and Portfolio value charts the trend. “Next 12 months” (bottom edge) previews net cash flow from the projection engine.

## Net Worth

The full balance sheet. Rows tagged “auto” are owned by another module (property, insurance, a brokerage account) and are edited there; everything else you add here directly.

![Net Worth](guide-screens/02-01-networth.png)

Net worth, assets and liabilities (37.5% of assets), the Composition bar split by class (property S$655,000, investments S$76,136, vehicle, cash, retirement, funds…), and a “What changed” card comparing two dates. It warns when the opening figure had to be rebuilt because net worth wasn’t recorded back then.

![Net Worth](guide-screens/02-02-networth.png)

“Net worth over time” records one point each time you open the page, so on a fresh install it shows “Building history” until there are two. Below it, every balance-sheet line: the flat and its mortgage as a liability, a manual car and car loan, CPF, cash, holdings and the policy at cash value.

---

# Cash Flow

## Cash Flow

A forward projection, not a ledger. Every module that knows about a future payment feeds a dated, signed amount here, tagged contracted, estimated or assumed so you can see which numbers are guesses.

![Cash Flow](guide-screens/03-01-cashflow.png)

The 5-year view: net +S$150,160 from S$330,810 expected income against S$180,650 expected expenses, shown as “Expected each year” bars for 2026–2031 with a stream legend (salary contracted, option income assumed, CPF mortgage portion estimated).

![Cash Flow](guide-screens/03-02-cashflow.png)

The running total is a separate chart on purpose (it dwarfs any single period). Below it: what drives each stream, and a “Locked / not yet accessible” section for money such as CPF or SRS that is projected but can’t be spent yet.

## Expenses

The actual dated ledger. Recurring rules auto-log their past occurrences as real, editable transactions and project future ones onto Cash Flow, so you enter a salary or rent once. Categories are a managed pick-list scoped by income vs expense.

![Expenses](guide-screens/04-01-expenses-categories.png)

Categories: one card per category with its month total. November 2026 shows S$892.22 of expenses (Household S$348.36, Allowance S$300, Mobile & Broadband S$65.40, Food & Drinks S$54.52) and S$20 of income.

![Expenses](guide-screens/04-02-expenses-calendar.png)

The finance calendar: a month grid with each day’s credit and debit totals (the 2nd is −S$321.55; the 9th has +S$20.00 and −S$10.98), with income, expense and balance cards beneath and the day’s transactions below that. “Show upcoming” adds projected rows.

![Expenses](guide-screens/04-03-expenses-stats.png)

Stats ranks the month by category with an expense/income toggle and a %/$ switch: Household 39.0%, Allowance 33.6%, Mobile & Broadband 7.3%, Food & Drinks 6.1%, Transport 5.8%.

![Expenses](guide-screens/04-05-expenses-spending-watch.png)

Spending watch answers “where should I look out for spending.” Average S$1,841.98 a month over Aug–Oct 2026, of which S$1,443.64 (78%) is variable and S$398.34 fixed; the variable table ranks Household, Food & Drinks and Shopping, judged against your own earlier months.

![Expenses](guide-screens/04-04-expenses-recurring.png)

Recurring rules: Salary (net of CPF) S$4,960 monthly from 2025-05-25, a mobile plan, home broadband and cloud storage. A rule can also be a fixed-count instalment plan, and “+ Add recurring item” creates one.

---

# Investments

## Stocks & ETFs

Average-cost holdings reconstructed from a buy / sell / dividend ledger, priced live via Yahoo Finance. Sub-tabs: Summary, Heatmap, Accounts, Holdings, Transactions and Splits.

![Stocks & ETFs](guide-screens/05-01-stocks-holdings.png)

Holdings: per-symbol quantity, allocation, average cost, price, market value, current return, dividends and yield. ES3.SI is S$20,220 (+18.41%), MSFT S$15,516 (+174.35%), D05.SI S$11,184 (+17.28%).

![Stocks & ETFs](guide-screens/05-02-stocks-transactions.png)

The Transactions ledger, newest first (narrowed to MSFT for this screenshot), mixing buys and auto-created dividend rows with their account. The 2026-06-15 buy of 12 shares at $0 is an RSU vest and the 2026-05-30 buy of 6 at $340 an ESPP purchase; the ledger lists both as plain buys, and when logged with that acquisition type they create the matching taxable-benefit income row in Expenses.

![Stocks & ETFs](guide-screens/05-03-stocks-summary.png)

Summary groups value by position and by market block, with brokerage totals of S$66,558 and S$9,578.

![Stocks & ETFs](guide-screens/05-04-stocks-heatmap.png)

Heatmap: tiles grouped by sector and coloured by today’s change; hovering a tile shows value, portfolio weight and total return.

![Stocks & ETFs](guide-screens/05-05-stocks-accounts.png)

Accounts regroups the same holdings by account: the margin brokerage at S$66,558 and the SRS account at S$9,578 (1,800 shares of ES3.SI).

![Stocks & ETFs](guide-screens/05-06-stocks-splits.png)

Splits is empty in the demo. Record a split once and every holding, dividend and historical value is restated through it; the transactions themselves are never rewritten.

## Dividends

Each dividend record auto-creates a per-account stock transaction (proportioned by shares held before the ex-date) and one Expenses income row. Declared-but-unpaid payouts feed the Cash Flow projection without yet showing as received.

![Dividends](guide-screens/06-01-dividends.png)

Summary: 28 dividend records, 0 upcoming payments, net dividends of S$1,338.64, totals by counter (ES3.SI S$611, D05.SI S$411.60, U11.SI S$170) and by currency.

![Dividends](guide-screens/06-02-dividends-heatmap.png)

Heatmap coloured by trailing yield, from U11.SI 4.5% and D05.SI 3.1% down to AAPL 0.2%.

![Dividends](guide-screens/06-03-dividends-records.png)

Records: ex-date, pay date, per-share amount, shares at ex-date, gross, withholding tax and net. The MSFT payout of 2026-10-15 is $0.83 × 23 shares, gross $19.09, 30% withholding $5.73, net $13.36.

## Options

Positions are rebuilt from the open / close / expire / assign / exercise lifecycle. Legs auto-group into a strategy by underlying and expiry, or by an explicit group, and an assignment or exercise auto-creates the matching stock trade.

![Options](guide-screens/07-01-options-positions.png)

An open short put on SPY (720, expiring 2026-12-05) expanded: breakeven 710.6, max profit $940, max loss −$71,060, and the payoff-at-expiration curve. “Roll position” and “Close position” act on the leg; three closed strategies sit collapsed below.

![Options](guide-screens/07-02-options-strategy.png)

A closed two-leg QQQ put credit spread (long 560 / short 570): the legs realised −S$272.09 and +S$449.02 for +S$176.93 net. Closed positions show their legs and P/L but no payoff chart.

![Options](guide-screens/07-03-options-transactions.png)

The transaction ledger with action, strike, expiry, contracts, premium and strategy grouping. The latest row is the SPY short put opened 2026-10-20 at $9.40.

![Options](guide-screens/07-04-options-summary.png)

Summary: per-underlying P/L and win rate (NVDA +S$411.23 at 100%, QQQ +S$176.93, SPY +S$886.84 with one open leg).

![Options](guide-screens/07-05-options-heatmap.png)

Heatmap of premium results by underlying. An open leg priced on a fallback mark is labelled as such, since there is no free option-price feed.

## Funds

Unit trusts and platform-held ETFs on a wrap or custodian account. Holdings are a periodic-statement snapshot (quantity, average cost, price) with no live NAV feed. Sub-tabs: Summary, Heatmap, Accounts, Holdings.

![Funds](guide-screens/08-01-funds-holdings.png)

Summary: market value S$25,043 against cost S$23,878, unrealised +S$1,165 (4.88%), with donuts by fund type, asset class and account above the holdings grouped by currency.

![Funds](guide-screens/08-02-funds-heatmap.png)

Heatmap by asset class, from World Technology +15.9% to the 20-year Treasury ETF −3.9%.

![Funds](guide-screens/08-03-funds-accounts.png)

Accounts: the wrap account’s cash bucket (S$25,043, 6 holdings, as of 2026-11-10) with “Update value”, which rescales prices to the custodian’s portal figure between monthly statements.

![Funds](guide-screens/08-04-funds-holdings-table.png)

Holdings table with fund type, asset class, funding source (cash or CPF), quantity, WAC, price and unrealised gain, e.g. Global Balanced Fund A 2,500 units at S$2.10 cost, S$2.35 price (+11.90%).

## Fixed Income

SGS bonds, T-bills, SSBs and P2P notes as a buy / coupon / redemption ledger against an instrument master. There is no live price feed, so value is accreted toward face value plus accrued interest, not marked to market.

![Fixed Income](guide-screens/09-01-fixedincome-holdings.png)

Holdings: a P2P note (S$3,000 face, flagged not government-guaranteed), a 6-month T-bill, a 2.75% 2034 SGS bond (S$10,036, next coupon S$137.50) and a 10-year SSB.

![Fixed Income](guide-screens/09-02-fixedincome-transactions.png)

The ledger: a S$20 coupon on the P2P note, a T-bill bought for S$9,890 against S$10,000 face, and a matured T-bill redemption of S$10,000.

![Fixed Income](guide-screens/09-03-fixedincome-summary.png)

Summary, the default tab: accreted value per instrument (the bond S$10,036 is 35.9% of fixed income), labelled “not a live market price”.

## Performance

Overall return (net profit ÷ capital deployed, not time-weighted) cut several ways. Per-year figures need a portfolio value at each year boundary, so early years can read “est” or “pending”.

![Performance](guide-screens/10-01-performance-assetclass.png)

By Asset Class: lifetime return +19.99%, net profit +S$24,484 on S$121,286 deployed. Stocks & ETFs +35.22%, Options +74.32%, Funds +6.19%, Fixed Income +2.09%.

![Performance](guide-screens/10-02-performance-year.png)

By Calendar Year: 2026 +S$41,857 on S$103,581 invested and 2025 −S$17,373. Return cells marked “est” rest on backfilled year-end snapshots.

![Performance](guide-screens/10-03-performance-position.png)

By Position: MSFT +S$9,905 (+175.14%), SPY options +62.61%, QQQ options +31.14%, U11.SI +22.94%.

![Performance](guide-screens/10-04-performance-dividends.png)

Dividends by Year: S$1,048.76 collected in 2026 (yield “est”) and S$331.90 in 2025 (yield “pending”).

![Performance](guide-screens/10-05-performance-costs.png)

Cost of Investing: 2026 stock fees S$22.69 plus option fees S$6.70 for S$29.38 in total; 2025 was S$48.41.

![Performance](guide-screens/10-06-performance-monthly.png)

Monthly Change: a gain/loss bar for each month, with November month-to-date at −S$1,889 (−1.80%) and a biggest-movers table below.

![Performance](guide-screens/10-07-performance-optionincome.png)

Option Income by Year: 2026 premium received S$3,463.91, premium paid S$772.62, fees S$6.70, net +S$2,684.60 across 9 transactions.

---

# Retirement

## CPF

Balances from an imported transaction history, a CPF LIFE estimator, and a contribution calculator that uses the same effective-dated rate table as the rest of the app. Importing is once per statement because the parser has no dedup.

![CPF](guide-screens/15-01-cpf-overview.png)

Overview: total S$41,292 (OA S$23,436, SA S$7,812, MA S$10,044, RA S$0), the FRS S$220,400 and ERS S$440,800, and the housing refund card (S$153,250 principal plus S$12,776 interest = S$166,026).

![CPF](guide-screens/15-02-cpf-life.png)

CPF LIFE estimator: Standard S$578, Basic S$506 and Escalating S$462 a month, with a warning that projected OA+SA at 55 (S$61,779) is S$158,621 short of the Full Retirement Sum.

![CPF](guide-screens/15-03-cpf-calculator.png)

Contribution calculator: enter a month’s ordinary wage and any bonus, or prefill from last month’s income, then Calculate for the employer/employee split against the wage ceilings. It is an empty form until you do.

![CPF](guide-screens/15-04-cpf-transactions.png)

The ledger, with “Add transaction”, “Set opening balance” and “Import statement”. One monthly contribution becomes OA, SA and MA rows (S$1,302 / S$434 / S$558 on 2026-10-26).

![CPF](guide-screens/15-05-cpf-rate-tables.png)

The rate table effective 2026-01-01: OW ceiling S$8,000, AW ceiling S$102,000, annual limit S$37,740, BHS S$79,000, and age-banded contribution percentages.

## Goals

Recomputed from the same runway inputs the Dashboard uses, plus one small assumptions blob. The FIRE number generalises “25× expenses” to a configurable withdrawal rate, and the stress test applies fixed percentage shocks to investments and funds only.

![Goals](guide-screens/16-01-goals.png)

FIRE number S$377,535 (S$15,101 a year ÷ 4%), liquid net worth S$153,370, progress 40.6% with S$224,165 to go, runway 10.2 years and a year-by-year projection.

![Goals](guide-screens/16-02-goals.png)

“Is the 4% rule right for you?” steps the suggested rate down as the horizon lengthens, and the drawdown scenarios show runway after −10%, −20% and −30% shocks (9.5, 8.8 and 8.1 years).

![Goals](guide-screens/16-03-goals.png)

Emergency fund: S$52,191 liquid cash covers 41.5 months against a 6-month target (S$7,551), a S$44,640 surplus. The same figures appear on the Dashboard tile. The Assumptions inputs follow.

---

# Planning

## Property

The amortisation schedule is rebuilt from principal, dated rates, CPF allocations, prepayments and refinances, so correcting a rate re-derives history exactly. A second model tracks the CPF accrued interest you must refund on a sale.

![Property](guide-screens/11-01-property-overview.png)

The demo HDB flat: purchase S$520,000, valuation S$655,000, equity S$332,888, mortgage outstanding S$322,112 with 253 of 300 instalments left, instalment S$1,735.82 at 3.10%.

![Property](guide-screens/11-02-property-schedule.png)

The repayment schedule, filtered to what remains. Instalment #48 (2026-12-14) is S$1,735.82: S$832.12 interest, S$903.70 principal, paid S$1,350 from CPF and S$385.82 in cash.

![Property](guide-screens/11-03-property-costs.png)

Costs: S$116,000 paid in cash and S$89,800 from CPF OA (S$205,800 upfront) across the downpayment, renovation, stamp duty and legal fees.

![Property](guide-screens/11-03-b-property-costs-if-sold.png)

“If you sold today”: a S$655,000 sale less the S$322,112 mortgage and a S$166,026 CPF refund (S$153,250 principal plus S$12,776 accrued interest) leaves S$166,862 in cash.

![Property](guide-screens/11-06-property-loan-terms-rates.png)

Loan terms: S$364,000 over 25 years, rate periods of 2.60% then 3.10%, and CPF S$1,350 a month. Prepayments sit alongside; a rate change recalculates the instalment over the remaining tenure.

![Property](guide-screens/11-07-property-refinance-events.png)

Refinance events are modelled separately from a repricing. None are recorded here; adding one re-amortises from that date over a fresh tenure.

![Property](guide-screens/11-04-property-comparables.png)

Comparable transactions from HDB’s published resale data, fetched on demand: 22 same-street, same-flat-type sales averaging S$1,114,131. Treat it with care. These are real transactions for a different block, far above the demo’s S$655,000, and “Use as valuation” is a deliberate, separate action.

![Property](guide-screens/11-05-property-cpf-runway.png)

CPF OA runway: starting from a S$23,436 OA balance and assuming no further contributions, the OA is projected to run out around May 2028.

## Insurance

Sum assured is coverage, not net worth. Only a policy’s cash value reaches the balance sheet. The protection gap is sized per risk as a lump sum, a monthly benefit or a ward tier.

![Insurance](guide-screens/12-05-insurance-summary.png)

Summary: cash value S$14,250, death cover S$810,000 (marked “NOT an asset”), premiums S$7,040 a year (S$6,560 cash plus S$480 from CPF), with donuts by insurer.

![Insurance](guide-screens/12-01-insurance-policies.png)

Five policies: Early Critical Care, Income Shield, Shield Plus (Private), Smart Saver Endowment 20 (cash value S$14,250) and Term Protect 25 (death cover S$750,000).

![Insurance](guide-screens/12-02-insurance-gap.png)

Protection gap: death cover S$810,000 against a need of S$876,939 (short S$66,939, 92% covered), TPD short S$126,939, critical illness short S$64,720, disability income S$3,500 against S$3,959 a month.

![Insurance](guide-screens/12-02-b-insurance-gap-needs.png)

Scrolling down: the remaining risk cards and the “Your needs” inputs that size them. Long-term care counts CareShield Life as a resource, and hospitalisation is reported as a ward tier rather than a dollar figure.

![Insurance](guide-screens/12-03-insurance-premiums.png)

Premiums: upcoming dated premiums over a 1 to 20-year window, starting 2027-05-24 with the endowment at S$3,600, split into S$6,560 cash and S$480 CPF a year.

![Insurance](guide-screens/12-04-insurance-projection.png)

Premium Projection by age to 99: S$7,040 a year at ages 37–46, falling to S$3,440 at 47 and S$2,800 at 56 as policies end.

## Estate

Readiness lives on your profile record; everything else is derived. US estate-tax exposure is computed only for non-resident aliens, walking current US-situs holdings through an effective-dated IRC §2001(c) table.

![Estate](guide-screens/13-01-estate-readiness.png)

Readiness: will, will signed and witnessed, LPA and CPF nomination, each with a “last updated” date and a link to the will details.

![Estate](guide-screens/13-02-estate-exposure.png)

Exposure for a non-resident alien: confirmed US-situs holdings $15,307 (0.3× the $60k exemption), illustrative net tax $0, $27,320 classed safe and $35,949 across 10 holdings still needing classification.

![Estate](guide-screens/13-03-estate-situs.png)

Situs classifications: a curated ticker-to-situs pick-list (US-situs, non-US, gray). Anything unmatched stays “needs classification” rather than being assumed safe.

![Estate](guide-screens/13-04-estate-rates.png)

The effective-dated rate table: unified credit $13,000 and brackets from 18% at $0 to 40% at $1,000,000, correctable as the IRS revises it.

![Estate](guide-screens/13-05-estate-schedule.png)

Schedule of assets, fully derived: S$937,725 of current assets (including the flat at S$655,000 and CPF OA S$23,436) plus a S$810,000 insurance payout, which is death benefit here and the opposite of the cash value used for net worth.

![Estate](guide-screens/13-06-estate-will.png)

The will builder: add beneficiaries, executors, gifts and residuary shares, then “Generate Will (.docx)”. Everything is empty in the demo.

## Tax

A stateless Singapore income-tax estimator. Nothing is saved as “the” estimate; the baseline and each what-if scenario are separate calls to the same calculator. Brackets and reliefs are effective-dated tables you correct as IRAS updates them.

![Tax](guide-screens/14-01-tax-estimate.png)

Inputs prefilled from this year’s income-kind expense categories (Income S$55,800, Equity Compensation S$6,922, Interest, Investments) so you choose which count as employment income.

![Tax](guide-screens/14-02-tax-estimate-lower.png)

With no category ticked the Baseline is near-empty: S$0 tax on S$15,000 chargeable income, reliefs S$5,000. Above it, your CPF retirement top-up room is S$219,200.

![Tax](guide-screens/14-05-tax-baseline-with-income.png)

After ticking Income as employment and pressing Calculate: tax S$804.80 on S$43,640 chargeable income (1.4% effective, 7.0% marginal) after S$12,160 of reliefs. Nothing is saved.

![Tax](guide-screens/14-03-tax-dependants.png)

Dependants: one entity for parents, children, spouse and grandparents. Margaret Tan (parent, living with you, income S$3,000) passes the income test.

![Tax](guide-screens/14-04-tax-rate-tables.png)

Rate Tables for Year of Assessment 2025: overall relief cap S$80,000, parent relief S$9,000 / S$5,500, donation multiplier 250% and the bracket ladder.

---

# Manage

## Accounts

Three levels: institution → account → sub-account (a funding split within one account, each with its own ownership share). Renaming with “apply to past” edits the row; without it a new account is created.

![Accounts](guide-screens/17-01-accounts-summary.png)

Summary: configured cash of S$67,375 across 5 accounts, grouped as Bank, Brokerage, Retirement (SRS) and Credit, where the card shows S$2,072 owed.

![Accounts](guide-screens/17-02-accounts-institution.png)

By institution: Emerald Bank, Northstar Brokerage and Summit Wealth as the brands, each with its accounts, ownership, transaction counts and balances.

![Accounts](guide-screens/17-03-accounts-all.png)

The flat sortable table: account number, product type, transaction count and balance. A credit card shows its “outstanding balance” in place of cash.

![Accounts](guide-screens/17-04-accounts-transfers.png)

Transfers move cash between your own accounts, one row carrying both sides in their own currencies: a S$738.66 card payment, a S$3,500 SRS contribution and an SGD→USD conversion. No recurring transfers are set up.

## Profile

Stable personal facts other modules read: date of birth (drives CPF and runway age gates), tax residency and US-person status (gate the SRS relief cap and the estate-tax regime) and the legal name used on generated documents.

![Profile](guide-screens/18-01-profile.png)

The demo profile: Alex Tan, born 12 Apr 1990, Singapore Citizen, not a US person. The SRS note reads “first contribution 2025-10-05 → prescribed age 63, unlocks 2053-04-12”, derived from the ledger unless you enter an override.

## Automations

Watch an outside source (an IMAP mailbox, a Tiger Brokers account) and turn what it shows into staged records. Review-first is the default: matches land in an inbox and nothing touches the ledger until you approve. All three tabs are empty in the demo.

![Automations](guide-screens/19-01-automations-connections.png)

Connections: the credential-holding links to external accounts. Credentials are encrypted at rest and never returned by the API. None yet.

![Automations](guide-screens/19-02-automations-rules.png)

Rules match items by sender, subject, body or date and extract fields. A connection is needed first; rules can be exported and imported without credentials.

![Automations](guide-screens/19-03-automations-review.png)

The review inbox, where matched items wait for you to approve, edit or reject before anything is written.

## Settings

App-wide preferences and the managed pick-lists. Eight tabs: General, Currency, Sectors, Holidays, Retirement Age, CPF Types, Finance Assistant and Backup & restore.

![Settings](guide-screens/20-01-settings-general.png)

General: rows per page (shared by every table), theme, and a replay-tour button.

![Settings](guide-screens/20-02-settings-currency.png)

Currency: base currency, optional API keys for live prices (Twelve Data), option earnings (Finnhub) and physical gold (GoldAPI), and a currencies table with manual FX overrides.

![Settings](guide-screens/20-03-settings-sectors.png)

Sectors: a GICS-seeded pick-list with usage counts (Information Technology 7, ETF/Diversified 6, Financials 3).

![Settings](guide-screens/20-06-settings-holidays.png)

Holidays: the Singapore public-holiday calendar, synced from data.gov.sg and editable. It drives the “next business day” rule for mortgage payment dates.

![Settings](guide-screens/20-07-settings-retirement-age.png)

Retirement Age: the statutory schedule (62 before 1 Jul 2022, 63 from then, 64 from 1 Jul 2026), used to work out when SRS withdrawals become penalty-free. Correct it as MOM announces step-ups.

![Settings](guide-screens/20-08-settings-cpf-types.png)

CPF Types: each CPF transaction code (contribution, housing, interest, refund…) with a cash-treatment setting.

![Settings](guide-screens/20-04-settings-assistant.png)

Finance Assistant: choose Anthropic, OpenAI, DeepSeek or a local Ollama model (shown here, no key needed). The model acts only through the same tools a person would use.

![Settings](guide-screens/20-05-settings-backup.png)

Backup & restore: your data is one local SQLite file; export a JSON backup or import one at any time.

---

All your data lives in a single local SQLite file. Export a JSON backup any time from Settings → Backup & restore. There is no server and no account, and nothing leaves your machine.
