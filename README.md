# Retail Sales & Customer Analysis: Excel

An Excel project that takes a retail sales table of 17,422 orders through data exploration, preparation, analysis and visualisation.

## Project Overview
The workbook holds one table (`Retailtable`) of orders with customer gender, marital status, income band, revenue, order date, birth date and country. The work follows four stages: explore, prepare, analyse and visualise.

## Objectives
- Understand the size and shape of the data.
- Derive new fields (year, weekday, customer age, age band, customer value, customer name).
- Measure revenue by country, gender and age band.
- Present the results in charts.

## Tools Used
Microsoft Excel: Tables and structured references, `IFS`, `IF`, `SUMIFS`, `TEXT`, `YEAR`, `LOWER`, `CONCAT`, `PROPER`, `COLUMNS`, `ROWS`, `MIN`/`MAX`/`AVERAGE`, charts.

## Methodology
**Stage 1: Data exploration:** counted columns and rows; calculated minimum, maximum, total and average revenue.

**Stage 2: Data preparation:** added columns for
- Year and Year-Month (`yyyy-mm`)
- Weekday name
- Customer name (first and last name merged, lowercase)
- Customer age (order year minus birth year)
- Age band: 13 to 19 Teenager, 20 to 34 Young Adult, 35 to 49 Adult, 50 to 64 Seniors, 65+ Elderly
- Customer value by order revenue: up to 1,500 Casual Buyers, 1,501 to 2,500 Brand Seekers, above 2,500 Convinced Seekers

**Stage 3: Analysis:** revenue by country and gender, and revenue by age band, using `SUMIFS`.

**Stage 4: Visualisation:** three charts: Revenue by Country, Proportion of Revenue by Age Band, and Revenue by Gender in Each Country.

## Key Findings
> Recalculated from the full dataset. Currency is not stated in the file.

- **17,422** orders over **18 columns**, from **May 2011 to June 2014**.
- **Total revenue about 21.76 million**; average about 1,249 per order; range about 2.53 to 5,398.
- **Australia is the largest market** at about 7.10 million (about 33% of revenue), followed by Southwest (3.57M), United Kingdom (2.87M), Germany (2.49M), Northwest (2.40M) and France (2.25M).
- **Age band share of revenue:** Adults (35 to 49) about 47%, Seniors (50 to 64) about 36%, Elderly (65+) about 14%, Young Adults about 3%. No orders fall in the Teenager band.
- **Gender:** Male customers generate more revenue in Germany, United Kingdom, Canada and Northwest; France is the main market where female revenue is higher; Australia is close to even.
- **Customer value:** about 61% of orders are Casual Buyers (10,616), 29% Convinced Seekers (5,092) and 10% Brand Seekers (1,714).

## Recommendations
- Protect and grow Australia, the largest revenue source.
- Target the 35 to 64 age groups, which produce most revenue.
- Investigate why the Southeast, Northeast and Central regions contribute almost nothing.

## Limitations
- The country and gender table in the workbook totals about 20.69 million, not the full 21.76 million, because it leaves out Canada (about 1.07 million) and Central (under 1,000). Charts built from that table therefore omit Canada. Add those rows to the table and refresh the charts if you want them to match the full dataset.

## Data Note
The source table includes customer first and last names. It appears to be a training or sample dataset. Confirm this before making the repository public; if it is real customer data, remove the name columns first.

## Repository Structure
```
retail-sales-analysis-excel/
├── README.md
├── data/Retail_Sales_Analysis.xlsx
└── screenshots/
```

## Charts
![Revenue by Country](screenshots/revenue_by_country.png)

## Author
**Olumide Goodness**
