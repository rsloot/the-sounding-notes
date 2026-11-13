# Cheaper Car Insurance Is Flattering the Inflation Numbers: data notes

Article: [The Sounding](https://thesounding.substack.com), November 13, 2026.

"My arithmetic" marks anything I computed. CPI figures are CPI-U, U.S. city average, not seasonally adjusted unless noted.

## Sources at a glance

| Source | Series | Frequency | Range used |
|---|---|---|---|
| Bureau of Labor Statistics, CPI-U | Car insurance, maintenance and repair, core (IDs below) | Monthly | Car insurance 2008 to October 2026; maintenance and repair to October 2026, with history from 1947 via FRED |
| Bureau of Labor Statistics, CPI relative importance | Table 2, September 2026 release | Monthly release | Weights as of August 2026 |
| Bureau of Labor Statistics, Producer Price Index | Private passenger auto insurance | Monthly | 2018 to September 2026 |
| Bureau of Economic Analysis | Core PCE price index; car insurance and core PCE spending; NIPA Handbook chapter 5 | Monthly; annual | Core PCE 1960 to September 2026, set against BLS core CPI (CPILFESL) over the same span; annual 2018-2025 |
| Progressive | Form 8-K, Exhibit 99 | Monthly report | September 2026 |
| Federal Reserve | FOMC statements, September 16 and October 28, 2026 | Per meeting | Quoted from federalreserve.gov |

## Consumer prices (BLS)

Pulled from the [BLS API v2](https://api.bls.gov/publicAPI/v2/timeseries/data/) on 2026-11-09 and re-pulled on 2026-11-10 after the October CPI. The latest month is October 2026. The latest 12-month changes are September 2026's.

- Motor vehicle insurance, CUUR0000SETE: 846.102 in September 2026 and 854.597 in October 2026. 12-month change -4.98% in September and -5.13% in August.
- Annual declines in May-September 2026. The previous ones were in January-March 2021.
- Five-year change, September 2021 to September 2026: +49.4%.
- Peak 12-month change: +22.6%, April 2024.
- No index exists for October 2025, nor for November 2025 for motor vehicle insurance (the 2025 lapse in appropriations).

Seasonally adjusted motor vehicle insurance, CUSR0000SETE, monthly changes in 2026:

| Jan | Feb | Mar | Apr | May | Jun | Jul | Aug | Sep | Oct |
|---|---|---|---|---|---|---|---|---|---|
| -0.44% | -0.33% | -0.04% | +0.14% | -1.69% | -2.01% | -0.29% | -0.75% | +0.06% | +0.71% |

- September 850.388 vs December 2025 897.307: -5.2%. October 856.439: -4.55% vs December 2025.
- October's +0.712% is the largest monthly rise of 2026 (next largest April, +0.14%). I don't rank it over a longer span, because the October-December 2025 monthly changes cannot be computed and April 2025's +0.707% ties it at published precision.

Repair costs:

- Motor vehicle maintenance and servicing, CUUR0000SETD02: +7.78% over the 12 months to September.
- Motor vehicle repair, CUUR0000SETD03: +3.55% over the 12 months to September (published 3.5%). Three-month annualized, July-October: +12.3% (309.733 to 318.843). June-September: +12.8%. August 2025: +5.03% on the month (291.623 to 306.282).
- Motor vehicle maintenance and repair, CUUR0000SETD: +5.79% over the 12 months to September. Three-month annualized, July-October: +10.1% (460.185 to 471.387), the same as June-September.
- The maintenance-and-repair 12-month change peaked at +14.2% in January 2023, the highest since 1975 (15.5% in March 1975). Source: FRED CUUR0000SETD, monthly from 1947. Motor vehicle repair alone peaked at +23.1% the same month.
- All items less food and energy, CUUR0000SA0L1E: +2.56% over the 12 months to September (published 2.6%).

## Core excluding car insurance (my arithmetic)

- Relative importance from CPI Table 2, September 2026 release (weights as of August 2026): motor vehicle insurance 2.531, all items less food and energy 79.075.
- Car insurance share of core: s = 2.531 / 79.075 = 0.0320.
- Core excluding car insurance = (core change - s x insurance change) / (1 - s) = (2.56 + 0.032 x 4.98) / (1 - 0.032) = 2.81%.
- With s carried back to the September 2025 base (0.0345): 2.83%. Both are approximations, because the CPI's weights were updated in December 2025.
- Contributions to all-items inflation = relative importance x 12-month change, from the same Table 2: motor vehicle insurance -0.127 points, health insurance -0.074, telephone hardware, calculators and other consumer information items -0.051.
- Drag on core: 0.0320 x -4.98 = -0.16 points.

## The Fed's gauge (BEA and PPI)

- BEA prices car insurance in PCE from the PPI for private passenger auto insurance: [NIPA Handbook chapter 5](https://www.bea.gov/resources/methodologies/nipa-handbook/pdf/chapter-05.pdf), Table 5.B, line 94 (net motor vehicle and other transportation insurance: price = PPI for private passenger auto insurance; current dollars = premiums less normal losses), read 2026-11-09.
- PPI series: PCU5241265241261 (direct property and casualty insurers, private passenger auto; BLS, preliminary): 243.086 in September 2026 vs 242.465 in September 2025, +0.26%. August: +0.91%.
- BEA's handbook names the PPI but not the series ID. This series matches BEA's annual price index (FRED DTINRG3A086NBEA) within 0.12 points in every year 2018-2025, so the match is an inference from fit.
- A second BLS series, PCU9241269241261 (premiums for private passenger auto insurance), was -0.28% in September. Either way, close to flat. PCU9241269241262 is homeowners' insurance, not auto.
- PCE weight, 2025: FRED DTINRC1A027NBEA $110.5bn / DPCCRC1A027NBEA $18,579bn core PCE = 0.59% (my arithmetic).

## Core CPI vs core PCE (my arithmetic)

- Core PCE, PCEPILFE: +3.121% over the 12 months to September 2026. Core CPI, CPILFESL: +2.566%. Both seasonally adjusted. August: 3.034% vs 2.446%.
- Gap: -0.555 in September, -0.588 in August. The last gap that wide in that direction was June 2010 (-0.61). FRED, monthly, 1960-2026.
- Car insurance's share of the gap = 0.25 (CPI side) - 0.017 (PCE side: 0.00595 x (3.121 - 0.26) / (1 - 0.00595)) = about 0.23 points, or 0.25 using the 2.83% base-weighted figure. This treats BEA's monthly price as the PPI.

## Federal Reserve

- Target range raised to 3.75-4.00% at the September 15-16 FOMC meeting (12-0; FRED DFEDTARU/DFEDTARL, effective September 17), and held on October 28 (10-2), per the federalreserve.gov statements.
- The FOMC's 2% goal is defined on the PCE price index, not the CPI.

## Progressive

[Form 8-K, Exhibit 99](https://www.sec.gov/Archives/edgar/data/80661/000008066126000367/pgr202609ex99earningsrelea.htm), October 14, 2026, month of September 2026, via SEC EDGAR.

- Personal Lines vehicle businesses, which include special lines: agency combined ratio 88.6, direct 92.7. Year to date: 85.1 and 89.6.
- Net premiums written: +1% agency, +1% direct.
- Auto-only policies in force, September 30, 2026 vs September 30, 2025: agency 11,347k vs 10,630k (+6.7%), direct 16,848k vs 15,619k (+7.9%).
- Company-wide combined ratio: 90.0, vs 100.4 in September 2025.

## Forecast checks (my arithmetic)

The second forecast leg is that core CPI excluding car insurance runs at least 0.10 points above published core in every month from December 2026 through April 2027. The September 2026 gap was 0.25.

Method: seasonally adjusted CUSR0000SETE (BLS API, pulled 2026-11-11), treating seasonally adjusted 12-month ratios as approximating the published unadjusted changes, with core at 2.6%.

| Car insurance path from October 2026 | April 2027 gap | Leg |
|---|---|---|
| Holds October's level (856.439) | 0.22: April 2027 is -3.92% on April 2026 (891.373), and 0.032 x (2.6 + 3.92) / 0.968 = 0.22. Unadjusted (854.597 vs 894.315): -4.44%, gap 0.23 | Holds |
| Rises steadily by about 0.6% a month (about 0.66% with core at 3.0%) | 0.10 | Break-even |
| Rises 0.7% a month, October's pace | Below 0.10 from March 2027 | Fails |

- Holding October's level, the gap in each month from December 2026 through April 2027 is between 0.21 and 0.24.
- The leg depends on the path, not only the average. A rise concentrated in the winter can push March below 0.10 at an average under 0.6% a month.
- November 2026 cannot be computed, because car insurance has no November 2025 index.

## Prior work cited

Reported as published. Figures from these sources were not reproduced.

- actuary.info, "[Auto Rate Cuts Collide With a Severity Re-Acceleration](https://actuary.info/insights/auto-severity-reacceleration-rate-cuts-2026)," July 23, 2026.
- actuary.info, "[Auto Insurance CPI Falls 5.1% in a Year While Repair Costs Rise 5.2%](https://actuary.info/insights/cpi-motor-vehicle-insurance-august-2026-first-annual-decline-since-2021-repair-costs-rising)," September 23, 2026. Estimates the headline effect at about 0.14 points, and expects negative annual comparisons, with 2025 rates earning in through mid-2027. The "filings take a year to earn" quote was verified 2026-11-09.

## Next data

- Progressive's October monthly results: not filed on EDGAR as of 2026-11-11 (last 8-K October 14).
- November CPI, December 10, 2026: the next 12-month change for core.
- December CPI, January 2027: the next 12-month change for car insurance.
- The forecast is graded by the December 2026 through April 2027 CPIs (the leg on the gap) and the December 2027 CPI, released January 2028 (car insurance back above its year-earlier level).

## Corrections

None since publication.
