# AtliQ Hardwares — Sales & Finance Analysis

Excel (Power Query + Power Pivot + DAX) project on AtliQ Hardwares sales and P&L for fiscal years **2019–2021** (Sep–Aug, values in USD).

The question the reports answer:

> Sales multiplied — so why did 2021 still miss target, and why did gross margin fall?

---

## Snapshot

| Year | Net sales |
|------|-----------|
| 2019 | $87.5M |
| 2020 | $196.7M |
| 2021 | $598.9M |

- **2021 vs 2020:** +304.5%
- **2021 vs target:** −$54.9M (**−9.17%**)
- Divisions: **P & A** (parts & accessories), **PC**, **N & S** (networking & storage)

---

## Reports

### 1. Customer Performance
Net sales by customer for 2019 / 2020 / 2021 and 21 vs 20 %.

| Customer (2021) | Sales |
|-----------------|-------|
| Amazon | $82.1M |
| AtliQ Exclusive | $61.1M |
| Atliq e Store | $53.0M |
| Sage | $20.7M |
| Flipkart | $19.3M |

Large accounts grew ~200–350%. Extreme % figures (Nova, Chiptec) are small-base effects, not volume.

**Use:** separate scale customers from noisy growth percentages.

### 2. Market Performance vs Target
Country sales against the 2021 target.

- **India** $161.3M — largest market, still **−$9.6M (−5.6%)** vs target
- **USA** $87.8M — **−$10.2M (−10.7%)**
- South Korea $49.0M
- Canada and Germany ~**−12.7%** vs target

Almost every market grew and still missed plan.

**Use:** growth and target-setting are different problems.

### 3. P&L by Fiscal Year
Net sales, COGS, gross margin and GM% by division.

2021 net sales: P&A **$338.4M** · PC $165.8M · N&S $94.7M

| Division | GM% 2019 | GM% 2020 | GM% 2021 |
|----------|----------|----------|----------|
| N & S | 40.7% | 36.8% | 36.7% |
| P & A | 41.9% | 37.4% | 36.4% |
| PC | 41.5% | 37.4% | 36.3% |

**Use:** revenue won; mix / discount / cost ate margin in every division.

### 4. P&L by Market (2021)
- India: $161.3M sales, $51.6M GM, **32.0%** GM
- High GM, smaller books: Norway **48.2%**, Japan **46.5%**, UK **45.1%**
- Germany: **26.2%** GM (lowest among listed markets)

**Use:** volume markets are tighter on margin; high-margin markets are smaller.

### 5. P&L by Months
Same P&L cut by fiscal month (Sep–Aug) for each year, plus YoY net-sales %.

**Use:** see seasonality and the 2020→2021 jump without hiding it in yearly totals.

---

## What I built

1. **Power Query** — extract / clean / load, date table, fiscal month and quarter
2. **Power Pivot** — table relationships and extra tables in one model
3. **DAX** — sales, COGS, gross margin, GM%, YoY, vs-target measures
4. **Reports** — region / market / division / customer / FY filters; YoY highlighted so outliers show up fast

---

## Read this first

1. Sales went from $87.5M to $598.9M. P&A is the engine.
2. 2021 still landed **~9% under target**.
3. GM% slid from ~**41%** to ~**36%** in all three divisions.
4. Amazon + AtliQ’s own channels carry a large share of 2021 sales.
5. India and USA = volume. Japan, Norway, UK = margin.

---

## Files

| File | Report |
|------|--------|
| `Customer Performance Report.pdf` | Customer sales + YoY |
| `Market Performance VS Targets.pdf` | Country vs 2021 target |
| `P & L by Fiscal Year.pdf` | Division P&L by year |
| `P & L by Market.pdf` | Country P&L (2021) |
| `P & L by Months.pdf` | Monthly P&L by FY |

Add the `.xlsx` / data-model file here when you upload it.

---

## Stack

Excel · Power Query · Power Pivot · DAX
