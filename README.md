# The Weak Yen Squeeze on Coffee

How much of the rise in Japanese coffee prices comes from global coffee markets vs. the weak yen, and how long does it take for import costs to reach consumers?

## Why it matters

Japan imports nearly all of its coffee, and green coffee is traded in U.S. dollars. Since 2022, Japan has faced record global coffee prices and a historically weak yen at the same time. This project separates those two forces and traces how import costs flow through to store shelves and cafes, with a focus on Okinawa.

## Data

- **Japan Customs, Trade Statistics of Japan:** monthly green coffee imports (HS 0901.11), total and by origin country, 2010 to 2026
- **FRED (Federal Reserve Bank of St. Louis):** IMF Arabica and Robusta prices, and the yen to U.S. dollar exchange rate
- **Statistics Bureau of Japan (e-Stat):** Consumer Price Index for coffee items, and store prices in Sapporo, Tokyo, Kyoto, and Naha

Japanese-language data was translated to English by the author. See `DATA_NOTES.md` for definitions, units, and caveats.

## Project structure

- `data/raw/` original data files, unchanged
- `data/processed/` cleaned and merged data
- `notebooks/` analysis notebooks, numbered in order

## Status

In progress. Data collected and cleaned; analysis underway.

## Author

Rey Colongon
