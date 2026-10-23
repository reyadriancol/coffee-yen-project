# Japan Coffee Price Data: Notes and Translations

All data pulled October 22, 2026 from Japanese government sources and translated to English. Monthly, January 2010 to August 2026.

## 1. japan_coffee_cpi_2010_2026.csv (national Consumer Price Index)

Source: Statistics Bureau of Japan, 2025-base Consumer Price Index, long-term time series, item price indices, all Japan, monthly (e-Stat, statInfId 000040482945).

Index values: **2025 average = 100**. An index is not a price in yen. Use it to compare how prices changed over time.

| Column | Original Japanese label | Meaning |
|---|---|---|
| cpi_all_items | 総合 | Overall inflation, all goods and services |
| cpi_coffee_and_cocoa | コーヒー・ココア | Coffee and cocoa group |
| cpi_instant_coffee | インスタントコーヒー | Instant coffee |
| cpi_coffee_beans | コーヒー豆 | Coffee beans (regular ground coffee bought in stores) |
| cpi_coffee_beverage_A | コーヒー飲料Ａ | Ready-to-drink coffee, type A (Statistics Bureau splits it into two specifications) |
| cpi_coffee_beverage_B | コーヒー飲料Ｂ | Ready-to-drink coffee, type B (starts 2015) |
| cpi_cafe_coffee_coffee_shop | コーヒー（外食）Ａ | Coffee at a traditional coffee shop (kissaten) |
| cpi_cafe_coffee_self_service | コーヒー（外食）Ｂ | Coffee at a self-service chain (starts 2015) |

Blank cells mean the item was not tracked yet.

Note: the CPI was rebased from 2020 = 100 to 2025 = 100 with the August 2026 release. This file uses the new 2025 base.

## 2. japan_coffee_retail_prices_by_city_2010_2026.csv (actual store prices)

Source: Statistics Bureau of Japan, Retail Price Survey (trend edition), "Retail prices of major items by city" (e-Stat database, statdisp_id 0003421913).

Prices are in **yen**, average of surveyed stores in each city.

| City in file | Japanese |
|---|---|
| Sapporo | 札幌市 |
| Tokyo (23 wards) | 東京都区部 (特別区部) |
| Kyoto | 京都市 |
| Naha | 那覇市 |

| item_code | Item | Unit | What is surveyed (current specification) |
|---|---|---|---|
| 1921 | Instant coffee | per 100g | Nescafe Gold Blend, jar (80 to 90g) |
| 1922 | Ground coffee (regular coffee) | per 100g | Ground blend coffee in a bag (200 to 260g): UCC Gold Special, Grand Taste, or Chotto Zeitaku na Coffee-ten |
| 2162 | Cafe coffee, coffee shop | per cup | Hot coffee at a traditional coffee shop, dine-in (not self-service or coffee stands) |
| 2165 | Cafe coffee, self-service chain | per cup | Hot coffee, small size, at a self-service coffee chain, dine-in |

Item 2165 starts January 2015. Sapporo and Kyoto are blank for May 2020 (no data published, likely COVID closures).

**Retail prices are raw; the CPI is adjusted.** The CPI adjusts for specification changes like the bag sizes above. For the "how much did prices really rise" question, use the CPI. Use the city retail prices for the city comparison (is Naha cheaper? does it lag Tokyo?).

**Single-city monthly prices are noisy.** Ground coffee and instant coffee jump around from month to month because of store sales. Use 3 or 12-month averages for charts.
