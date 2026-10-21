# 🌍 Access to Drinking Water (2000-2020) - Excel Analysis

Analysis of global access to safe drinking water using WHO/UNICEF Joint Monitoring Programme (JMP) data, to measure progress toward **UN SDG 6 - Clean Water & Sanitation**.

Built during the **ALX Africa Data Analytics program**, in two parts.

---

## 🎯 Objective

Find out who has access to basic drinking water, where access is improving or declining, and which regions and populations are being left behind.

---

## 📘 Part 1 - Understanding the data (2020 snapshot)

**File:** `Part1_Water_Access_2020_Snapshot.xlsx`, covering 213 countries.

- Cleaned the dataset: converted numbers stored as text, replaced "NAN" text with empty cells, fixed broken formulas.
- Added calculated columns: population in millions, urban/rural shares and populations.
- Checked data consistency with a validation column, since the four service levels should add up to ~100%. It flagged 2 inconsistent countries, which were corrected or documented.
- Compared the dataset with the world population estimate (it covers 99.6% of the world's population).
- Produced descriptive statistics for all 12 access indicators (national, rural, urban).
- Compared access by income group.

**Key findings**
- Low-income countries average **63% basic access**, vs **99.6%** in high-income countries.
- In low-income countries, urban areas have **29.5 points more access** than rural areas, compared with a gap of only 1.2 points in high-income countries.

---

## 📈 Part 2 - Transforming the data (2000-2020)

**File:** `Part2_Water_Access_2000-2020.xlsx`, covering 231 countries with two records each.

- Checked year coverage and the gap between records per country (average 4.8 years).
- Calculated **Annual Rates of Change (ARC)** in basic access for national, rural and urban populations.
- Classified countries by full access, no change, decrease or increase, with a check that every country is counted.
- Calculated the rural vs urban ARC difference and its distribution.
- Added regions with a lookup and compared progress by region (summary table + bubble chart).

**Key findings**
- On average, access improves by **0.28 points per year nationally**, 0.48 in rural areas and 0.15 in urban areas.
- Rural access improved faster than urban access in **112 countries** (vs 23 the other way).
- **26 countries saw urban access decline.**
- **Sub-Saharan Africa** improves fastest (0.56 points/year), but only 2 of its 53 countries have full access. At the current rate, the region would only reach full access around **2080**.

---

## 🛠️ Tools & techniques

Excel · Google Sheets · data cleaning · IF / IFERROR / COUNTIFS / AVERAGEIF / SUMPRODUCT · INDEX/MATCH lookup · descriptive statistics · histograms · bubble chart

---

## 📁 Files

- `Part1_Water_Access_2020_Snapshot.xlsx`: Part 1 analysis
- `Part2_Water_Access_2000-2020.xlsx`: Part 2 analysis
- `data/Estimates_of_the_use_of_water_2020.csv`: raw 2020 dataset (Part 1)
- `data/Estimates_of_the_use_of_water_2000-2020.csv`: raw 2000-2020 dataset (Part 2)
- `data/Regions.csv`: country → region classification

Each workbook has an **About** sheet explaining the sheets, the cleaning steps and every column.

---

## 🙏 Credits

Case study: **ALX Africa Data Analytics program**. Data: WHO/UNICEF Joint Monitoring Programme (JMP).
