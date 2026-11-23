# Data notes: Only One in Four Businesses Uses AI. That's the Bull Case.

Article: [The Sounding](https://thesounding.substack.com/p/only-one-in-four-businesses-uses), November 23, 2026.

An opinion piece: the market spent the week of November 16-20 selling short-term news (the trees) while the government's own count of AI adoption (the forest) rose to a record. "My arithmetic" marks anything I computed. Figures were pulled November 20-23, 2026.

## Sources at a glance

| Source | Series | Frequency | Range used |
|---|---|---|---|
| U.S. Census Bureau, Business Trends and Outlook Survey (BTOS) | National estimates (`National.xlsx`), question 7: AI use in the previous two weeks; question 28: expected use in the next six months; questions 8-10 | Fortnightly | Cycles 202524-202623 (reference periods Nov 3-16, 2025 to Oct 19-Nov 1, 2026). Pulled 2026-11-20 |
| U.S. Census Bureau, BTOS | Employment-size-class estimates (`Employment Size Class.xlsx`), question 7 | Fortnightly | Cycles 202524 and 202623. Pulled 2026-11-23 |
| Yahoo Finance; Nasdaq historical quotes | Daily closes and opens: NVDA, AMD, MU, RSP, ^GSPC, ^SOX, ^VIX | Daily | Nov 11-23, 2026 |
| ICE BofA US High Yield Index option-adjusted spread (FRED `BAMLH0A0HYM2`) | Spread over Treasuries | Daily | Jan 2025-Nov 19, 2026 |
| Cboe VIX (FRED `VIXCLS`; Yahoo Finance and CNBC for the Nov 20 intraday high) | Close and high | Daily | Jan 2025-Nov 20, 2026 |
| U.S. Treasury, daily real yield curve | 5-year real (inflation-protected) par yield | Daily | Feb 27 and Nov 20, 2026 |
| SEC filings | Nvidia 8-Ks (Nov 12 and Nov 23, 2026), Nvidia Q3 FY27 results (Nov 17), Nvidia 10-Q (filed Aug 26, 2026) | Event | 2026 |

## The Census survey (BTOS)

Question 7 asks whether the business used AI "in any of its business functions" in the previous two weeks. Census broadened the wording in late 2025 (its "AI Question Wording Updates" page, Dec 3, 2025); the first release under that wording is the series start below, so earlier releases are not comparable and are not used. From the collection that began Oct 19, 2026 (cycle 202622), the questionnaire calls the technology "Super Intelligence or SI (formerly referred to as Artificial Intelligence or AI)" and adds new examples. The share using it dipped at that release (24.6% to 24.2%) rather than jumping.

Estimates are shares of businesses: a business with two employees counts the same as one with 20,000.

| Cycle | Reference period | Published | Used AI in previous two weeks |
|---|---|---|---|
| 202524 | 2025-11-03 to 2025-11-16 | 2025-12-04 | 17.3% |
| 202525 | 2025-11-17 to 2025-11-30 | 2025-12-18 | 17.2% |
| 202526 | 2025-12-01 to 2025-12-14 | 2025-12-31 | 17.8% |
| 202601 | 2025-12-15 to 2025-12-28 | 2026-01-15 | 17.7% |
| 202602 | 2025-12-29 to 2026-01-11 | 2026-01-29 | 18.2% |
| 202603 | 2026-01-12 to 2026-01-25 | 2026-02-12 | 18.9% |
| 202604 | 2026-01-26 to 2026-02-08 | 2026-02-26 | 17.5% |
| 202605 | 2026-02-09 to 2026-02-22 | 2026-03-12 | 18.2% |
| 202606 | 2026-02-23 to 2026-03-08 | 2026-03-26 | 18.9% |
| 202607 | 2026-03-09 to 2026-03-22 | 2026-04-09 | 19.1% |
| 202608 | 2026-03-23 to 2026-04-05 | 2026-04-23 | 19.8% |
| 202609 | 2026-04-06 to 2026-04-19 | 2026-05-07 | 19.8% |
| 202610 | 2026-04-20 to 2026-05-03 | 2026-05-21 | 19.5% |
| 202611 | 2026-05-04 to 2026-05-17 | 2026-06-04 | 20.6% |
| 202612 | 2026-05-18 to 2026-05-31 | 2026-06-18 | 20.6% |
| 202613 | 2026-06-01 to 2026-06-14 | 2026-07-02 | 20.6% |
| 202614 | 2026-06-15 to 2026-06-28 | 2026-07-16 | 21.7% |
| 202615 | 2026-06-29 to 2026-07-12 | 2026-07-30 | 21.5% |
| 202616 | 2026-07-13 to 2026-07-26 | 2026-08-13 | 21.8% |
| 202617 | 2026-07-27 to 2026-08-09 | 2026-08-27 | 22.4% |
| 202618 | 2026-08-10 to 2026-08-23 | 2026-09-10 | 23.2% |
| 202619 | 2026-08-24 to 2026-09-06 | 2026-09-24 | 23.8% |
| 202620 | 2026-09-07 to 2026-09-20 | 2026-10-08 | 23.8% |
| 202621 | 2026-09-21 to 2026-10-04 | 2026-10-22 | 24.6% |
| 202622 | 2026-10-05 to 2026-10-18 | 2026-11-05 | 24.2% |
| 202623 | 2026-10-19 to 2026-11-01 | 2026-11-19 | 25.0% |

- Up from 17.3% to 25.0% over the 26 releases (about 50 weeks; the 2025 shutdown left no exact year-earlier reading). My arithmetic: about 7.7 percentage points a year.
- The series dipped six times (cycles 202525, 202601, 202604, 202610, 202615 and 202622); each dip was reversed at the next release.
- Expected use in the next six months (question 28), cycle 202623: 28.2%. Every business is asked, so this includes the 25.0% already using AI.
- "Do not know" on question 7: 9.6-9.8% in the four releases before the questionnaire change, 13.9% in cycle 202622 and 13.3% in cycle 202623.
- Employees using generative AI for work tasks (question 8, new from cycle 202622): 27.6% in cycle 202623.
- Headcount (question 9, asked only of businesses that answered yes to question 7 or 8), cycle 202623: 87.4% no change over the past six months, 7.3% increased, 2.4% decreased, 2.9% did not know.

AI use by employment size class (question 7):

| Employees | Cycle 202524 (Nov 3-16, 2025) | Cycle 202623 (Oct 19-Nov 1, 2026) |
|---|---|---|
| 1 to 4 | 17.0% | 23.4% |
| 5 to 9 | 15.5% | 25.3% |
| 10 to 19 | 17.8% | 27.8% |
| 20 to 49 | 18.7% | 28.1% |
| 50 to 99 | 20.7% | 33.1% |
| 100 to 249 | 23.7% | 35.3% |
| 250 or more | 30.5% | 44.0% |

Standard errors in cycle 202623: 3.74 points for 250 or more, 0.88 points for 1 to 4.

## Chart

"A record share of US businesses now uses AI." Question 7 above, plotted at the end of each reference period, with the questionnaire change marked. Source: Census BTOS national estimates. Chart: The Sounding.

## Markets (my arithmetic unless noted)

- Nvidia: $173.73 (Nov 11 close) to $125.53 (Nov 20 close, confirmed on Nasdaq historical quotes), -27.7%; it closed lower six days running, Nov 12-19. At 24.1 billion shares (cover of the 10-Q filed Aug 26, 2026, as of Aug 21), about $1.16 trillion of market value.
- Nov 23: Nvidia opened at $167.04 (Yahoo daily bar and CNBC), 33.1% above Friday's close, about $1.00 trillion of market value. Yahoo's 9:30 a.m. one-minute bar shows $163.00 (+29.9%), so the article says "roughly a third." The same morning Micron opened about 16% higher and a semiconductor ETF about 15%.
- Micron: $811.30 to $594.51 (Nov 11 to Nov 20 closes), -26.7%.
- Invesco S&P 500 Equal Weight ETF (RSP): $222.65 to $207.44, -6.8%.
- AMD: -7.72% to $489.19 on Nov 19 (CNBC).
- S&P 500: 6,910.39 on Nov 20, 11.6% below its Oct 6 record close of 7,818.93, so in correction.
- VIX: closed at 35.89 on Nov 20; intraday high 40.03 (Yahoo Finance and CNBC). Before Nov 20 it last closed above 35 on Apr 4, 7, 8, 10 and 11, 2025.

## Credit and rates

- ICE BofA US High Yield option-adjusted spread: 3.52 percentage points on Nov 19, 2026, up from 3.20 on Nov 12; the widest since 3.53 on May 9, 2025. On the five April 2025 days the VIX closed above 35 it was 4.45, 4.61, 4.57, 4.42 and 4.26. The Nov 20 value had not been published when the article was written.
- 5-year real Treasury yield (Treasury daily real yield curve): 1.11% on Feb 27, 2026, the last trading day before the war with Iran began on Feb 28, and 2.53% on Nov 20, 2026 (my arithmetic: 2.28 times).
- December rate-hike odds: CNBC, Nov 20: "Traders are still pricing in about a 92% chance of a quarter percentage point rise in the fed funds rate in December" (CME FedWatch, Friday morning).

## The trees: events and statements

- Nvidia 8-K, filed Nov 12, 2026: the board accepted Jensen Huang's resignation on Nov 11; Colette Kress, chief financial officer, became interim chief executive.
- The New York Times, Oct 29, 2026, on Huang's ties to Alice Huang, a former Megaspeed executive, as reported by TechCrunch (timeline, Nov 13).
- The Wall Street Journal, Nov 17, 2026, as reported by Reuters: the SEC was examining whether Nvidia's disclosures misled investors. Neither the SEC nor Nvidia has confirmed it.
- Hunterbrook, "AMD Has Its Own China Problem," Nov 19, 2026 (Hunterbrook's fund disclosed a short position). AMD to CNBC: the claims "misrepresent AMD's business practices and relationships"; AMD "complies with applicable US export control laws and regulations."
- Commerce Department interim final rule, 91 FR 74970, effective Nov 19, 2026: license requirements for advanced chips to Indonesia, Malaysia, Singapore, Thailand and Brazil, with an exemption for buyers headquartered in the United States subject to reporting; and for data centers abroad supplying significant compute to companies headquartered in Country Group D:5 or Macau.
- Nvidia Q3 FY27 results, Nov 17, 2026: outlook "not assuming any Data Center compute revenue from China."
- Nvidia 8-K, Nov 23, 2026: Huang reinstated as President, CEO and director by unanimous board vote. "In the process of reaching its decision, the Board received input from senior levels of the United States government, and based on that input, the Board is confident that Mr. Huang's reinstatement poses no national security risk." The independent committee's investigation "will proceed to conclusion."

## Capacity quotes (earnings calls)

- Microsoft (Amy Hood), Oct 28, 2026: "Customer demand continues to exceed available supply." Same call: roughly three-quarters of the quarter's capital spending went on short-lived assets, primarily CPUs and GPUs.
- Microsoft (Hood), Jul 29, 2026: "if the demand environment changes, you just slow down what is, in fact, the largest component and the driver of COGS."
- Alphabet, Oct 28, 2026: "given the supply-constraint environment, we started utilizing third-party compute capacity."
- Amazon (Andy Jassy), Q3 2026 call: "almost as fast as we install capacity, customers are gobbling it up."

## Other figures

- International Federation of Robotics, World Robotics 2026 (Sep 24, 2026): China installed 354,000 industrial robots in 2025, 59% of global installations.
- Epoch AI, "The plunging price of thought" (Emberson and Roodman, Sep 22, 2026): the price of a given level of performance has fallen "about 47% per quarter since 2023, or 13x per year." MIT FutureTech finds that the cost of running frontier models is rising, which the article notes.
- National Conference of State Legislatures, "Does your state offer data center tax incentives" (Apr 9, 2026): 38 states offer them, and all waive sales taxes on essential data center equipment.
- Democrats won both chambers of Congress on Nov 3, 2026 (AP); the new Congress convenes Jan 3, 2027.

## Prior work credited

- Goldman Sachs Research (Ryan Hammond), Apr 16, 2024: the AI trade in phases, ending with Phase 4, "AI-productivity gains" for companies across industries.
- Axios, Mar 20, 2026, "AI chip smuggling signals strong Chinese demand," on smuggling as a demand signal.

## Forecast check

1. In the Census BTOS release scheduled for Feb 18, 2027 (cycle 202703, reference period Jan 18-31, 2027), the share of businesses using AI will be 27% or higher, about where the past year's trend points. Below 27%: a slowdown. At or below 25.0%: wrong.
2. In their January-February 2027 earnings calls, Alphabet, Amazon and Meta will each guide to more capital spending in 2027 than in 2026, and Microsoft (fiscal year ending June) will be the only one of the four to signal, by its April 2027 call, slower capital-spending growth for the fiscal year starting July 2027. Wrong if any of the three guides to less, or if Microsoft does not.

## Corrections

None since publication.
