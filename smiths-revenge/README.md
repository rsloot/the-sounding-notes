# Smith's Revenge: data notes

Article: [The Sounding](https://thesounding.substack.com/p/smiths-revenge), November 19, 2026.

The piece is a thought experiment: it argues from a premise about a world where AI makes cognitive skill cheap. The sources below are the ideas it builds on, the evidence it cites as signals, and the prior work it credits. "My arithmetic" marks anything I computed. Checked 2026-11-11.

## Sources at a glance

| Source | Series | Frequency | Range used |
|---|---|---|---|
| Bureau of Labor Statistics, Occupational Employment and Wage Statistics (OEWS) | National files, annual median wages by detailed occupation | Annual (May surveys; fourth-quarter surveys in 2001 and 2002) | May 2005-May 2025 in the text; 2001-2025 in the chart. Pulled 2026-11-06 |
| Census Bureau, American Community Survey | 2024 1-year PUMS, civilian employed, person-weighted | Annual | 2024 |
| Adam Smith, *The Wealth of Nations* (1776) | Book I, Chapters II and X | n/a | Checked against Project Gutenberg #3300 |
| Marginal Revolution Podcast (Mercatus) | "Compensating Differentials and Selective Incentives" | n/a | November 4, 2025 |

## Adam Smith

- *The Wealth of Nations* (1776), Book I, Chapter X, Part I: the five circumstances; the public executioner; honour "makes a great part of the reward of all honourable professions," and they are "generally under-recompensed."
- Book I, Chapter II: the philosopher and the street porter ("habit, custom, and education").
- Checked against Project Gutenberg #3300.

## The podcast

- Marginal Revolution Podcast (Mercatus), "Compensating Differentials and Selective Incentives," November 4, 2025.
- The skill-scarcity point is Alex Tabarrok's.
- Tyler Cowen on segmentation, and on compensating differentials mattering less in a more tech-like economy.

## Prior work credited

- Matthew Parris, "Will AI make bricklayers better-paid than barristers?" *The Spectator*, September 26, 2024.
- Lawrence Lundy-Bryan, "Dirty Work: The Return of Blue Collar," State of the Future (Substack), June 4, 2025.
- Anton Korinek, Charles I. Jones, Szymon Sacher, Tess Cotter and Peter McCrory, "Economic Scenarios for Transformative AI," The Anthropic Institute Working Paper No. 2026-02, September 2026.
  - Extreme scenario, 2030: the cognitive wage is 11.5% below the no-AI path, and the wage in all other occupations is 33.6% above it in Table 3 ("34 percent" in the introduction).
  - Labor in those jobs is "comparatively scarce"; in the long run there is "a single wage in the model."
  - The scenarios "are not predictions." The model ends in 2030 and excludes robotics.
  - Found via Alex Tabarrok, "AI, Redistribution, and the Size of the Pie," Marginal Revolution, September 14, 2026.

## Wages (BLS OEWS)

National files, May 2005-May 2025, pulled 2026-11-06. Annual medians.

| Occupation (SOC code) | May 2019 | May 2025 | Change |
|---|---|---|---|
| All occupations | $39,810 | $50,980 | +28.1% |
| Refuse and recyclable material collectors (53-7081) | $37,840 | $49,690 | +31.3% |
| Interpreters and translators (27-3091) | $51,830 | $60,170 | +16.1% |
| Janitors (37-2011) | | | +34.3% |
| Cashiers | | | +39.0% |
| Retail salespersons | | | +40.2% |
| Tellers | | | +37.8% |

The cashier, retail salesperson and teller changes are the fact-checker's computations from the same files.

Translator-to-collector median ratio (my arithmetic):

- 1.22 (2005), 1.38 (2012), 1.37 (2019), 1.21 (2025).
- 1.21 is the lowest of all 21 annual files from May 2005 to May 2025, and of all 25 values from 2001 shown in the chart. The fourth-quarter 2001 and 2002 surveys give 1.34 and 1.35; May 2003 and 2004 give 1.39 and 1.31.
- In dollars, the 2025 gap ($10,480) exceeded the gaps in 2005-2009, 2013-2015 and 2022.

Same-pay comparison (my arithmetic): of 133 other detailed occupations with identical codes in May 2019 and May 2025 and a May 2019 median within 10% of collectors' $37,840, 32 rose faster and 101 slower. Their median gain was +27.3%.

Computer programmers (15-1131 through May 2018, 15-1251 from May 2019), employment:

- 230,470 (May 2018), 199,540 (May 2019), 132,740 (May 2022), 92,230 (May 2025).
- The May 2019-2020 estimates mix 2010 and 2018 SOC codes, and BLS does not encourage OEWS time-series comparisons.

## Chart

"Translators' pay lead over garbage collectors hits a 25-year low." Median yearly pay of interpreters and translators divided by that of refuse and recyclable material collectors, yearly surveys 2001-2025 (the ratio series above). Source: BLS OEWS national files. My calculation.

## AI studies

- Brynjolfsson, Li and Raymond, "Generative AI at Work," *Quarterly Journal of Economics* 140(2), 2025. About a 15% average gain; 30% for less-skilled and less-experienced agents; little effect for the most skilled.
- Noy and Zhang, *Science* 381:187-192 (2023). 453 professionals; inequality between workers decreased.

## Immigrant shares (ACS)

Census Bureau, American Community Survey 2024 1-year PUMS, civilian employed, person-weighted (my computation):

- Roofers (Census code 6515): 54% foreign-born.
- Janitors and building cleaners (4220, broader than OEWS 37-2011): 30%.
- All workers: 18%.

## Automated garbage trucks

Metro Nashville Department of Waste Services, news release, May 27, 2026 ("single-operator collection").

## Forecast check

In the Labor Department's May 2035 wage survey (published around spring 2036), the median annual wage for refuse and recyclable material collectors will be at least as high as the median for interpreters and translators. If the 2028 occupation codes split or merge interpreters and translators, the test applies to their successor occupations. Wrong if collectors are still below translators. In May 2025 the collectors' median was $49,690 and the translators' $60,170.

## Corrections

None since publication.
