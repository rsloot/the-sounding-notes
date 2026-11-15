# Your Electric Bill Is the AI Boom's Backstop: data notes

Article: [The Sounding](https://thesounding.substack.com), November 17, 2026.

"My arithmetic" marks anything I computed.

## Sources at a glance

| Source | Series | Frequency | Range used |
|---|---|---|---|
| Energy Information Administration, EIA-860M Preliminary Monthly Electric Generator Inventory | "Planned" and "Canceled or Postponed" sheets | Monthly editions | January 2016-2020, July 2017-2021, January 2024-2026, March 2025, July 2025, July 2026 and September 2026 (September released 2026-10-23); the chart also uses January 2021-2023 |
| Energy Information Administration, EIA-860 | 2025 final Utility file, "Entity Type" (released 2026-09-10) | Annual | 2025 |
| Entergy Corporation | Form 10-Q, third quarter 2026 (filed 2026-11-02, EDGAR) | Quarterly | As of September 30, 2026 |
| Evergy, Inc. | Form 10-Q, third quarter 2026 (filed 2026-11-05, EDGAR) | Quarterly | As of September 30, 2026 |
| Duke Energy | Third-quarter 2026 earnings call, November 5, 2026 (transcript, The Motley Fool) | Quarterly | As stated on the call |

EIA-860M files: eia.gov/electricity/data/eia860m/. Pulled 2026-11-06 and independently re-downloaded (sha256-identical) by a separate fact-check pass. The January 2017-2026 and September 2026 editions were downloaded again on 2026-11-15 to rebuild the chart, and every share below reproduced.

## Planned gas capacity (EIA-860M)

- Gas = "Natural Gas Fired Combined Cycle" and "Natural Gas Fired Combustion Turbine". All planned status codes (P, L, T, U, V, TS, OT).
- Nameplate MW, except January 2016 (net summer only; 30.8% utility share on that basis). On a summer basis the 2017-to-2026 shares are 30.6% and 69.2%.
- Sector is EIA's plant-level sector of the operating entity: "Electric Utility" vs "IPP CHP"/"IPP Non-CHP". Small commercial and industrial CHP is excluded. Shares are utility/(utility+IPP): my arithmetic.
- EIA's classification follows the operator, so a jointly owned plant counts entirely toward its operator's side.

Totals:

- January 2017: 70.11 GW (utility 20.99, IPP 48.16).
- September 2026: 70.14 GW including Fermi America; ex-Fermi 58.46 (utility 41.12, IPP 17.25). Including Fermi, the utility share is 58.7%.
- Totals include 0.96 GW (2017) and 0.09 GW (2026) of commercial and industrial units, excluded from the shares and the chart.

Utility share by edition (ex-Fermi; my arithmetic):

| Edition | Utility share |
|---|---|
| January 2017 | 30.3% |
| January 2018 | 29.3% |
| January 2019 | 28.1% |
| January 2020 | 29.5% |
| January 2021 | 26.0% |
| January 2022 | 29.9% |
| January 2023 | 31.6% |
| January 2024 | 39.0% (pipeline 16.58 GW) |
| January 2025 | 59.8% |
| January 2026 | 69.7% |
| July 2026 | 72.6% |
| September 2026 | 70.4% |

Investor-owned share: joins the operator's Entity ID to the EIA-860 2025 final Utility file "Entity Type" (released 2026-09-10), utility/(utility+IPP) basis: 20.6% (Jan 2017) and 49.4% (Sep 2026 ex-Fermi). 2025 types applied to all editions.

Other utility types (September 2026): Tennessee Valley Authority 3.89 GW, cooperatives 5.28 GW, public-power systems 3.02 GW.

Planned operation year 2028-2030: 75.5% of planned gas nameplate (Sep 2026, including Fermi; my arithmetic).

Status (Sep 2026, including Fermi): U+V 14.8%, U+V+TS 18.3% (TS = construction complete, not yet in commercial operation), P 55.8%. Utility P share 41.3% ex-Fermi.

Entergy subsidiaries (Sep 2026): 15.75 GW of planned gas, 38% of the 41.12 GW utility total; ex-Entergy utility share 59.5%.

Fermi America (Sep 2026): 157 planned gas units, 11.68 GW, 128 of them dated December 2030. No rows in the January 2026 file.

July-to-September 2026 editions: nothing newly canceled; 2.25 GW added to Planned; 4.88 GW of dates slipped, 2.11 GW of them Fermi's.

Duke Energy coverage gap: the Planned sheet has no Duke Energy gas units in any state in the January 2025, January 2026, July 2026 or September 2026 editions (Duke's planned rows there are solar and batteries only), and no planned gas units at all in North or South Carolina in the January and September 2026 editions. On its November 5, 2026 earnings call Duke said it is "advancing regulatory filings specific to natural gas generation with more than 5 gigawatts under construction in the Carolinas and Indiana and another 5 gigawatts in development." The inventory therefore undercounts at least this utility's gas build, so on this count the utility shares above are if anything understated (the file may also miss independent projects: no SoftBank or SB Energy entity is on the September 2026 Planned sheet), and the cancellation shares cannot see Duke's projects. I have not established why the units are missing.

## Cohorts and cancellations (my arithmetic)

- Cohorts match plant ID + generator ID across editions. Units re-numbered at commissioning can be missed; this affects the 2017-18 windows, not the recent ones.
- "Due" = units whose own planned date falls inside the 18-month window.
- IPP cancellation share by cohort (planned gas nameplate on the Canceled or Postponed sheet 18 months later): 40.0% (Jan 2024 cohort, by Jul 2025), 25.4% (Jan 2025, by Jul 2026), 17.9% (Mar 2025, by Sep 2026). Utility: 0.0% in all three.
- Utility share canceled in the 2016-2020 windows: 3.5% to 17.7%.
- Utility units due online within the window and operating by its end: 65%, 65% and 75% in the three recent cohorts; 61% to 100% across the 2016-2020 windows. About a quarter of the Mar 2025 cohort was still in planning at Sep 2026.
- Utility units that appeared on the canceled sheet only temporarily are not counted as cancellations: OG&E Tinker (Jan 2025 edition only, later operating) and AECI Ripley (Feb-May 2026, back on Planned).
- Utility additions to the sheet, Jan 2024-Sep 2026: Arizona Electric Power Cooperative, Apache Station GT7 and GT8, 51.1 MW each.
- Independent additions to the sheet, Jan 2024-Sep 2026: 4.013 GW, including Coronado Power Ventures (1,282 MW), two FGE Texas plants (743 MW each) and Gila Bend (900 MW).

## Company filings

- Entergy Q3 2026 10-Q, filed 2026-11-02 (EDGAR): seven combined-cycle units, 5,278 MW, "approximately $12.9 billion," in service 2030-2031, for Evest LLC, a subsidiary of Meta Platforms. Certification application filed with the Louisiana Public Service Commission in March 2026; hearing held October 2026; settlement with LPSC staff and one intervenor recommending certification; decision expected December 2026. Customer protections, and "a guaranty from Meta Platforms, Inc."
- Evergy Q3 2026 10-Q, filed 2026-11-05: "primarily large load customers with expected load in excess of 75 MWs," $8.9 billion remaining performance obligations, 15-year weighted-average remaining term, as of September 30, 2026.

## Press and prior work credited

Reported as published.

- Bloomberg, "Data-Center Pullback in US May Shield Real Economy From AI Bubble," November 6, 2026 (headline only).
- Reuters, "Nasdaq posts biggest daily drop in 19 months on fears of AI regulations," November 5, 2026.
- Latitude Media, September 24, 2026 (59% vs 4%).
- Rystad Energy, via Oilprice.com, March 1, 2025: utility-sector planned gas, excluding IPPs, "from 6 GW in late 2023 to a staggering 17.5 GW currently, the highest since 2017."
- Brookings (Klaus and MacCarthy), October 30, 2025: gas plants that "typically operate for 30 years" serving data centers with "10- or 15-year contracts." The same contract-versus-plant-life point on the Entergy-Meta case: Krati Kaushik on Substack, October 27, 2026.
- Duke Energy, Smith Energy Complex combustion turbine: WUNC, September 21, 2026 (certificate denied as "premature"; "$584 million"; questions on data-center use and cost). Duke's response from its November 5, 2026 earnings call: "Our Smith CPCN that we filed was denied by the commission," and it would "reevaluate" after the resource-plan decision. The NCUC order itself was not reachable.
- SoftBank: TechCrunch, "SoftBank's billion-dollar loss may have put a cap on AI's natural gas ambitions," November 12, 2026: a $7.1 billion quarterly loss announced Tuesday, November 10, "over half of that stemming from losses related to power-generating equipment," after deposits on "more than 13 gigawatts of turbines, almost 50% more than it needed."
- Global Energy Monitor release, August 25, 2026, and Axios, August 26, 2026.
- RMI, August 6, 2026.
- CoBank, July 28, 2026.
- Nemadji Trail Energy Center (a combined-cycle plant) cancellation per WPR (October 29, 2026), WDIO and Northern News Now (October 28), POWER (November 3) and Sierra Club (October 2026), including the 625 MW and $1 billion figures, which I have not verified against the PSC docket. Its absence from the 860M planned sheet was checked by the fact-check pass across editions from January 2019 to September 2026.

## Forecast checks

Graded on EIA-860M editions through March 2027 (due around late May 2027):

- Utility gas newly added to the Canceled or Postponed sheet relative to the January 2026 edition: less than 1 GW (wrong at 2 GW or more).
- IPPs, Fermi included, add more to that sheet than utilities.
- Utility share ex-Fermi stays at or above 65% (wrong below 60% in any edition).
- If the LPSC approves Entergy's units in December, they should move off "approvals not initiated" by the February 2027 edition.

## Next data

- EIA-860M October 2026 edition, due November 24, 2026 (per EIA's release schedule), and later editions; all shares will be recomputed on the newest file.
- Louisiana Public Service Commission decision on Entergy's units, December 2026.

## Corrections

None since publication.
