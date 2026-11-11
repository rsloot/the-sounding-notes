# The Cities That Built the Most Now Have the Least Shelter Inflation: data notes

Article: [The Sounding](https://ryansloot.substack.com), November 11, 2026.

"My arithmetic" marks anything I computed. All CPI figures are CPI-U, not seasonally adjusted.

## Sources at a glance

| Source | Series | Frequency | Range used |
|---|---|---|---|
| Bureau of Labor Statistics, CPI-U | National and metro indexes (IDs below) | Monthly; metro all-items bimonthly for 20 areas | September 2021 to October 2026; Houston shelter from 2016 for a seasonal check |
| Census Bureau, Building Permits Survey | CBSA annual and year-to-date files, estimated units | Annual; January to September year to date | 2021-2025; January-September 2025 and 2026 |
| Census Bureau, population estimates | Vintage 2025 CBSA estimates | Annual | 2020 and 2025 |
| Census Bureau, Housing Vacancy Survey | 2026 Table 4, rental vacancy | Quarterly | 26Q1-26Q3 average |
| Federal Reserve, FOMC statements | September 16 and October 28, 2026 | Per meeting | Quoted verbatim, federalreserve.gov |

## Consumer prices (BLS)

- Source file: the BLS CPI-U flat file [cu.data.0.Current](https://download.bls.gov/pub/time.series/cu/cu.data.0.Current) (file dated 2026-10-19, data through September 2026), pulled 2026-11-06 and independently re-downloaded (byte-identical) in a separate fact-check; spot-checked against the [BLS API v2](https://api.bls.gov/publicAPI/v2/timeseries/data/).
- All figures in the article are not seasonally adjusted 12-month changes unless stated.
- U.S. all items CUUR0000SA0: 3.74% (336.940 / 324.800). Shelter CUUR0000SAH1: 3.22%. Energy CUUR0000SA0E: 20.45%. All items less food and energy CUUR0000SA0L1E: 2.56%.
- Metro shelter CUUR[area]SAH1, September 2026 vs September 2025.
- Houston, all items less food and energy, CUURS37BSA0L1E: 285.868 (August 2026) vs 286.389 (August 2025).
- September 2022 shelter 12-month changes: Houston 7.37% (CUURS37BSAH1), New York 3.45% (CUURS12ASAH1); BLS API, pulled 2026-11-09.
- No October 2025 index exists for the metro shelter series (confirmed via the BLS API, 2026-11-09), so no October 2026 12-month metro changes are published.
- Metro all-items indexes are bimonthly for 20 areas, so headline reference months are August or September 2026. Shelter, rent and owners' equivalent rent are monthly for all 23 areas. Energy is monthly for 22 (BLS discontinued Baltimore energy, CUURS35ESA0E, after May 2026).
- The October 2025 carry-forward and April 2026 catch-up are described in the BLS [2025 shutdown CPI FAQ](https://www.bls.gov/cpi/additional-resources/2025-federal-government-shutdown-impact-cpi-faq.htm). The size of the effect on December 2026 12-month changes is my estimate, not BLS's.

### October 2026 CPI (released November 10)

BLS API v2, pulled 2026-11-10, not seasonally adjusted. No October 2025 index exists for any series below, so there are no October 12-month changes.

- Houston, less food and energy, CUURS37BSA0L1E: 289.258 in October vs 285.868 in August, +1.19% (bimonthly). Above August 2025 (286.389) by 1.00% and December 2025 (284.755) by 1.58%.
- Houston shelter, CUURS37BSAH1: 335.157 in October vs 334.413 in September, +0.22%. Versus December 2025 (331.827), +1.00%. Versus September 2025 (334.905), +0.08%.
- New York shelter: 503.244, +0.41% on the month.
- Dallas shelter, CUURS37ASAH1: 354.466, +0.13% on the month.
- Phoenix shelter fell 3.06% on the month.
- Houston shelter's October-to-December change ranged from -0.75% (2024) to +1.45% (2022) in 2016-2024, with no consistent seasonal dip, so holding October's level is a neutral baseline (my arithmetic).

## Contributions and variance shares (my arithmetic)

- Contributions use the BLS December 2025 relative-importance tables (U.S.: shelter 35.625, energy 6.383) and metro weights from the same release. National contributions of about 1.31 points (energy) and 1.15 points (shelter) are approximate because weights drift.
- Variance shares = covariance of each contribution with headline inflation, divided by the variance of headline inflation across metros.
- Energy and "other" shares were computed with Baltimore's energy imputed from regional August changes (5.0-6.5% and 43.8-45.2%) or with Baltimore dropped (5.6% and 41.2%; shelter 53.2%).

## Building permits and population (Census)

- Permits: Census Building Permits Survey CBSA annual files 2021-2025 and year-to-date files cbsa2609y / cbsa2509y (January-September), estimated units, pulled 2026-11-06 from the [BPS directory](https://www2.census.gov/econ/bps/). cbsa2609y was re-downloaded 2026-11-09 and was byte-identical (md5).
- The October year-to-date file had not been posted as of 2026-11-11. September permits are preliminary and will be revised.
- Per-1,000 rates use 2020 population. With 2025 population the leaders are Phoenix 43.9, Houston 43.6 and Dallas 42.8; correlations move by 0.03 or less.
- Population: Census Vintage 2025 CBSA estimates.
- Rental vacancy: Census Housing Vacancy Survey 2026, Table 4, average of 26Q1-26Q3.
- BLS CPI areas are mapped to Census CBSAs. Urban Hawaii and Urban Alaska are mapped to Honolulu and Anchorage, which is why the 21-metro results (excluding those two) are the primary ones.
- Philadelphia: the full 10-year tax abatement applied to permits issued by December 31, 2021, stepping down thereafter (Philadelphia Inquirer, Blumgart and Briggs, December 7, 2022). The 2021 CBSA BPS file shows 25,427 units in buildings with five or more units.

## Correlations and per-capita figures (my arithmetic)

- All correlations, partial correlations, per-capita and per-new-resident figures (Philadelphia about 1.03, Houston about 0.47 on 2021-2025 permits) are my arithmetic.

## Forecast checks (my arithmetic)

The December 2026 forecast legs, checked against the October 2026 indexes for the 21 metro shelter series (CUUR[area]SAH1, BLS API v2, pulled 2026-11-10). Each December 2026 12-month change is estimated against that metro's December 2025 index. Permits per 1,000 are as in the main ranking, which reproduces the September correlation of -0.68.

| Path to December | Correlation | Houston rank (lowest = 1) | Six big cities above 3.5% |
|---|---|---|---|
| Every metro holds its October level | -0.69 | 3rd, at 1.00% (Phoenix -0.62%, Tampa 0.78%, Atlanta 1.09%, Dallas 1.32%) | 5 of 6 (Philadelphia 1.83% the exception) |
| Each metro keeps its July-October pace two more months | -0.62 | 5th, at 1.80% (Phoenix, Tampa, Atlanta, Dallas lower) | 5 of 6 |
| Each metro keeps its September 12-month pace | -0.69 | 3rd | 5 of 6 |

## Federal Reserve

- FOMC statements of September 16 and October 28, 2026, federalreserve.gov, quoted verbatim.
- The FOMC's 2% goal is defined on the PCE price index, not the CPI.

## Prior work cited

Reported as published; figures from these sources were not reproduced unless stated.

- Admir Kolaj, "[Where Inflation Burns Hottest: A U.S. Metro View of the Latest Price Surge](https://economics.td.com/us-metro-inflation)," TD Economics, June 25, 2026 (read 2026-11-11). Describes the metro shelter divergence, with no permits, construction or supply link.
- Mark Vitner, "The Map Has Flipped: Dispersion, Regulation and a New Municipal Math," Piedmont Crescent Capital, August 2026.
- CRE Daily, "Midwest Leads 2026 US Multifamily Rent Growth as Sun Belt Lags," June 20, 2026 (Yardi Matrix).
- Cotality, "Single-family rent growth steadies as Midwest leads and Sun Belt softens," June 18, 2026.
- Dvorkin and Marks, Federal Reserve Bank of St. Louis, November 26, 2024.
- Miles, Journal of Economics and Business (2026), [doi 10.1016/j.jeconbus.2026.106330](https://doi.org/10.1016/j.jeconbus.2026.106330).
- Westpac IQ, Bustamante and Sharma, "Beyond housing, regional underlying inflation is remarkably similar," September 21, 2026 (trimmed-mean inflation, capital cities, since 2000).
- Inman, Pipitone, "Rents are falling (almost) everywhere. What's happening?" July 14, 2026. Inman's own analysis of Realtor.com's June 2026 Rent Report table: median asking rents, 46 of the 50 largest metros, June 2026 rent growth against 2025 multifamily permits per 1,000 residents. Inman notes it is not necessarily statistically significant. A web signal, not reproduced.

## Next data

- Census October year-to-date permits (cbsa2610y): not posted as of 2026-11-11.
- November CPI, December 10, 2026: the next 12-month metro shelter changes.
- FOMC meeting, December 8-9, 2026.
- December CPI, January 13, 2027: grades the forecast.

## Corrections

None since publication.
