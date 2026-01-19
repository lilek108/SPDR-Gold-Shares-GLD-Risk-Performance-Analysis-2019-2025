# SPDR Gold Shares (GLD): Risk & Performance Analysis 2019-2025

# Project Background

**GLD (SPDR Gold Shares)** is an exchange-traded fund (ETF) that tracks the price of gold, one of the most widely used commodities in the world. Launched to provide investors with a cost-effective and liquid way to gain exposure to gold, GLD represents ownership in physical gold stored in secure vaults. Gold, which is traditionally considered a very stable asset, is often included in diversified investment portfolios to reduce overall risk, although it is considered less profitable.

Recently, due to increasing economic instability, geopolitical tensions, and market uncertainty, investor demand for safe-haven assets like gold has grown significantly. This rising interest prompted an analysis of GLD’s historical returns, volatility, correlations, and risk-adjusted performance to assess its relevance and potential role in investment portfolios today.

Key analysis questions:

Returns and Performance:
  * How has GLD performed historically in terms of **returns**?
  * Has the price of GLD shown consistent **growth or large fluctuations**?

Volatility and Risk:
  * What is the historical **volatility** of GLD?
  * How large are the **drawdowns**?
  * How including GLD would affect the **risk-adjusted performance** of a portfolio?

Correlation:
  * How **correlated** is GLD with major equity and bond indices?

An interactive **Power BI dashboard** used in this analysis can be found [here](https://app.powerbi.com/view?r=eyJrIjoiMWRiODBkODgtODljZS00OTc3LWJlNGUtNzA3NDU2MDNjNWYwIiwidCI6ImUwMGRkY2RmLTFlMGYtNGJlNS1hMzdhLTg5NGE0NzMxOTg2YSIsImMiOjh9&pageName=620982043be653777d90).

Historical price data used in this analysis were obtained using the **Python Yahoo Finance (yfinance) library**.

# Data Structure and Overview

Besides **GLD**, for additional correlation analysis, the project also incorporates the **US Dollar Index (DXY)**, the **10-Year US Treasury Yield (TNX)**, and the **S&P 500 Index (GSPC)** to better understand GLD’s behavior relative to major financial benchmarks.

The final  dataset structure as seen below consists of four tables: *gld_clean, DXY_clean, TNX_clean, GSPC_clean,* with a total row count of **1762 records**. All tables have the similar structure with the exact same columns and data types:

<img width="1051" height="708" alt="image" src="https://github.com/user-attachments/assets/23f9e933-79de-40ba-b8bd-d971dae3202d" />

<img width="392" height="319" alt="image" src="https://github.com/user-attachments/assets/7626e6b5-557e-42f9-a9db-7f7a7a624bc4" />

<br>
<br>

# Executive Summary

GLD has shown **strong price and returns growth** in recent years, accompanied by **elevated volatility**. Despite its **long-term stability and diversification benefits**, historical returns have not risen proportionally with price, indicating that the recent surge is an **unusual**, period-specific phenomenon rather than a structural trend. While **cyclical within-year fluctuations** provide **moderate short-term trading opportunities**, the recent performance should be interpreted with **caution**, as it brings **higher uncertainty** and **downside risk** rather than guaranteed future gains.

# Insights 

**1. Sustained Long-Term Growth with a Recent Acceleration Phase**

Over the past five years (2021-2025), GLD demonstrated strong and stable price appreciation, with its price increasing from **$151** to **$417**, resulting in a total cumulative return of **226.64%** and an annualized return of **18.44%**. These figures indicate a **sustained upward trend** in both price and returns, supporting the view of gold as a resilient long-term investment over the analyzed period.

<img width="900" height="439" alt="image" src="https://github.com/user-attachments/assets/e7d49aba-87c5-44ce-8a57-075631e53ed8" />

<img width="135" height="207" alt="image" src="https://github.com/user-attachments/assets/2997ae3a-f719-4a61-93b2-1db51e1b2d9f" />

<br>
<br>

To provide a more detailed analysis and to account for major global events (particularly those of 2020) the deeper analysis covers a broader time horizon (not the traditional 5 years timeframe) spanning from 2019 to the end of 2025, which reveals distinct growth phases. Between 2019 and 2023, GLD experienced moderate growth with **noticeable cyclicality**: the price increased from a low of approximately **$120** in early 2019 to a peak of **$194** in August 2020, after which it moved in cyclical patterns until the end of 2023. During this four-year period, the cumulative return reached **57.56%** an annualized return was **9.54%**, reflecting steady but relatively moderate performance.

<img width="899" height="438" alt="image" src="https://github.com/user-attachments/assets/e42e174d-7af0-46b9-aa70-643126d106df" />

<img width="147" height="211" alt="image" src="https://github.com/user-attachments/assets/b841530d-dd13-4960-90f4-26f0611da7eb" />

<br>
<br>

In contrast, the period from early 2024 to the end of 2025 was characterized by a **significant acceleration** in price dynamics. GLD’s price rose sharply to **$417**, while the lowest observed price during this period declined only to **$184** in February 2024. As a result, the cumulative return and annualized return over just two years amounted to **107.31%** and **44.09%** respectively, highlighting a substantial increase in both price growth and return momentum compared to the previous phase.

<img width="896" height="444" alt="image" src="https://github.com/user-attachments/assets/c9fe2586-91d6-4890-aea8-2343e9485291" />

<img width="139" height="210" alt="image" src="https://github.com/user-attachments/assets/51b823ad-db53-4d1f-878d-9d84f30b653b" />

<br>
<br>

**2. Short-Term Return Profile and Changing Trading Attractiveness of GLD**

From 2019 to 2023, GLD exhibited **moderate potential for short-term trading**, with pronounced **within-year fluctuations in its 90-day rolling mean returns** offering tactical opportunities. However, the **absence of a consistent upward trend**, combined with an average daily return of **0.07%** and a Sharpe ratio of **0.64**, indicates **limited appeal for long-term investment**.

<img width="748" height="237" alt="image" src="https://github.com/user-attachments/assets/241a8486-12dc-4b77-898e-c44c2cd22827" />

<img width="745" height="79" alt="image" src="https://github.com/user-attachments/assets/cacb044e-9efc-4f48-82e4-a5c79080c5c8" />

<br>
<br>

Over the 2019–2025 horizon, the average Sharpe ratio increased to **1.17**, but this improvement is **largely driven by the most recent two years** rather than by a gradual enhancement of return dynamics across the entire period. Return distributions **remained approximately normal**, with **larger deviations** observed in 2020 and 2025, primarily associated with major global and geopolitical events (COVID-19 and the U.S. presidential transition respectively).

<img width="748" height="235" alt="image" src="https://github.com/user-attachments/assets/88e051c7-22a6-4eba-99d0-03350071dfeb" />

<img width="748" height="83" alt="image" src="https://github.com/user-attachments/assets/28b525e9-63ef-4b34-b478-9b88504db365" />

<img width="510" height="296" alt="image" src="https://github.com/user-attachments/assets/e129b206-32ee-412a-a9df-ac6134c81232" />

<img width="505" height="109" alt="image" src="https://github.com/user-attachments/assets/1a25685e-15c9-45cd-b5d1-21eb69ddc678" />

<br>
<br>

During 2024–2025, GLD’s **short-term trading attractiveness increased materially**: the average daily return rose to **0.15%**, the share of positive-return days **increased**, and the Sharpe ratio climbed to **2.51**, indicating substantially **better risk-adjusted performance**. This implies that while GLD’s high average return over the full six-year period is **predominantly explained by the strong performance of the last two years**, so likely the improvement represents a **period-specific enhancement** rather than a persistent shift in the asset’s short-term return profile.

<img width="750" height="239" alt="image" src="https://github.com/user-attachments/assets/20f58f10-e6b7-4071-ae87-d42324db9c49" />

<img width="746" height="79" alt="image" src="https://github.com/user-attachments/assets/cc75f060-01ce-46ea-9416-bea3e3f72a56" />

<br>
<br>

**3. Volatility Changes and Historical Drawdowns**

Overall, the **1‑year rolling volatility increased** over the past **five years**. This growth, however, was **not consistent**. Volatility stood at approximately **18%** at the beginning of 2021, declined to a **minimum of 11.18%** in early 2024, and later reached a **peak of 21.59%** in November 2025. In contrast, the drawdown chart demonstrated an **overall downward trend with smaller fluctuations**, reaching its maximum in late 2022. For the entire period, the annualized volatility was **15.75%**, while the **maximum** drawdown reached **–22.00%**.

<img width="787" height="382" alt="image" src="https://github.com/user-attachments/assets/94bf4bda-81a8-4f70-83f0-f675328358dc" />

<img width="779" height="377" alt="image" src="https://github.com/user-attachments/assets/834a86b1-d666-443a-99eb-bc74e1a740e9" />

<img width="121" height="182" alt="image" src="https://github.com/user-attachments/assets/168ec70a-5ea4-4629-a451-62fff4392a11" />

<br>
<br>

Between 2019 and 2023 (**2020–2023*** for 1‑year rolling volatility due to missing 2018 data), the 1‑year rolling volatility followed a mostly **cyclical pattern**. It reached a **low of 11.72%** in late 2023, similar to levels seen in early 2020 and late 2021–early 2022. The **peak** occurred in fall 2020 at **21.40%**, with a smaller upswing in early 2023. Drawdowns over 2019–2023 were also **cyclical**, with larger fluctuations after 2019 and the **deepest drawdown** occurring in fall 2022. Annualized volatility for 2019–2023 was **14.93%**, slightly below the 2020–2025 value.

<img width="778" height="378" alt="image" src="https://github.com/user-attachments/assets/be37f098-2ece-4ba3-8a36-8637764db611" />

<img width="771" height="374" alt="image" src="https://github.com/user-attachments/assets/7fa80b6d-b1da-425a-8e1e-3e0e4028cb21" />

<img width="124" height="185" alt="image" src="https://github.com/user-attachments/assets/9f963bd3-d049-4810-9262-d09809044762" />

<br>
<br>

During 2024–2025, the 1‑year rolling volatility increased markedly, rising from roughly **12%** to a **peak of 21.59%**. Combined with the annualized volatility of **17.58%**, this reflects a clear **intensification of price instability** over the period. Despite the heightened volatility, the drawdown pattern **remained cyclical and relatively contained**, with a **maximum** drawdown of only **10.13%**. This limited downside movement indicates that the elevated volatility was driven primarily by the **speed of GLD’s price appreciation** rather than by substantial price declines.

<img width="766" height="378" alt="image" src="https://github.com/user-attachments/assets/2b5048ca-d685-4c27-aa6a-4a20b3a7bba9" />

<img width="764" height="382" alt="image" src="https://github.com/user-attachments/assets/cddbf87a-3055-4aaf-aabe-011a1432fed0" />

<img width="119" height="186" alt="image" src="https://github.com/user-attachments/assets/66820fac-6b55-4898-be6b-ef6901ffc5ea" />

<br>
<br>

**4. Correlations Overview and Diversification Attractiveness**

The correlation matrix for GLD, TNX, GSPC, and DXY indicates that GLD returns exhibit **no strong correlation** with the returns of the other assets. The strongest observed relationship is a **moderate negative correlation** with **DXY** (–0.35). GLD also shows a **weak negative correlation** with **TNX** (–0.26) and an **essentially insignificant positive correlation** with **GSPC** (0.11). Overall, the limited correlation between GLD and the selected assets underscores its **attractiveness as a diversifying component** within a portfolio.

<img width="1130" height="519" alt="image" src="https://github.com/user-attachments/assets/0da17876-11be-4759-805d-20ff7f68968b" />

<br>
<br>

# Recommendations:

 * Be **cautious** when considering GLD as a **long‑term investment** aimed at stable returns, given its rapid and **disproportionate price growth** over the past two years and its relatively **low risk‑adjusted performance** during the preceding five‑year period.
 * Take into account the **potential for short‑term**, intrayear trading opportunities in GLD, driven by the **pronounced fluctuations in the 90‑day rolling mean return** and the recent **increase in volatility**.
 * Highlight the attractiveness of GLD as a **diversifying component** within a portfolio, given its **limited correlation** with major equity and bond indices.

