# Global Interplay Among Military Expenditures, Educational Investments, Prosperity, and Happiness

## Project Overview

This project analyzes how education spending, military spending, GDP per capita growth, prosperity, and happiness vary across countries by World Bank income group from 2011 to 2021.

The project uses Python for data cleaning and Tableau for visual analytics. Countries are grouped into High income, Upper middle income, Lower middle income, and Low income categories using World Bank classifications.

The main goal is to understand how countries balance education and military spending, and how those spending patterns are associated with economic growth, prosperity, and happiness outcomes.

## Project Objective

Governments face difficult choices when dividing national budgets between education, military spending, and other public services.

This project explores whether countries that spend more on education or military priorities show different patterns in:

- GDP per capita growth
- Prosperity score
- Happiness score
- Income group performance
- Country-level outliers

The analysis does not claim direct causation. It studies patterns and associations across countries and income groups.

## Research Questions

1. How do education spending, military spending, and GDP per capita growth differ across countries by World Bank income group?

2. Is higher education spending as a percentage of GDP associated with stronger GDP per capita growth, prosperity, and happiness outcomes?

3. How is military spending as a percentage of GDP related to GDP per capita growth across different income groups?

4. Among countries with similar income levels, how do education and military spending priorities differ, and how are these priorities associated with prosperity and happiness outcomes?

5. Which countries stand out as high education spenders, high military spenders, high growth countries, or prosperity and happiness outliers?

## Tools and Technologies Used

- Python
- Pandas
- NumPy
- Tableau
- Excel
- GitHub

## Data Sources

This project uses public datasets from World Bank, World Happiness Report, SIPRI-based World Bank military indicators, and Legatum Prosperity Index.

| Dataset | Source | Direct Link | Used For |
|---|---|---|---|
| World Bank Country and Lending Groups | World Bank | https://databankfiles.worldbank.org/public/ddpext_download/site-content/CLASS.xlsx | Country code, region, and income group classification |
| GDP Current US$ | World Bank | https://api.worldbank.org/v2/en/indicator/NY.GDP.MKTP.CD?downloadformat=csv | Total GDP by country and year |
| GDP Per Capita Growth Annual % | World Bank | https://api.worldbank.org/v2/en/indicator/NY.GDP.PCAP.KD.ZG?downloadformat=csv | GDP per capita growth by country and year |
| Education Spending as % of GDP | World Bank | https://api.worldbank.org/v2/en/indicator/SE.XPD.TOTL.GD.ZS?downloadformat=csv | Education spending as a share of GDP |
| Military Expenditure Current US$ | World Bank, based on SIPRI Military Expenditure Database | https://api.worldbank.org/v2/en/indicator/MS.MIL.XPND.CD?downloadformat=csv | Military spending in current US dollars |
| Military Expenditure as % of GDP | World Bank, based on SIPRI Military Expenditure Database | https://api.worldbank.org/v2/en/indicator/MS.MIL.XPND.GD.ZS?downloadformat=csv | Military spending as a share of GDP |
| World Happiness Report | World Happiness Report | https://www.worldhappiness.report/data-sharing/ | Happiness score and supporting happiness indicators |
| World Happiness Report Figure 2.1 Data | World Happiness Report | https://files.worldhappiness.report/WHR25_Data_Figure_2.1.xlsx | Happiness score and explained factors |
| Legatum Prosperity Index | Legatum Prosperity Index | https://index.prosperity.com/about/resources | Prosperity score and country-level prosperity ranking |
| Legatum Prosperity Rankings | Legatum Prosperity Index | https://index.prosperity.com/rankings | Prosperity ranking and country comparison |

## Final Cleaned Datasets

The final Tableau workbook uses seven cleaned datasets:

| Cleaned File | Description |
|---|---|
| Income group.csv | Country code, standardized country name, region, and World Bank income group |
| GDP_Current_USD.csv | GDP in current US dollars by country and year |
| GDP_PC_Growth.csv | GDP per capita growth annual percentage by country and year |
| Education.csv | Education spending as percentage of GDP by country and year |
| Military.csv | Military spending in current US dollars and military spending as percentage of GDP |
| Happiness.csv | Happiness score and supporting happiness indicators by country and year |
| Prosperity.csv | Prosperity score by country and year |
| Combined_Tableau_Analysis_2011_2021.csv | Combined validation dataset used to verify country-year matching |

## Repository Structure

```text
Global-Interplay-Among-Military-Expenditures-Educational-Investments-and-Prosperity-Rates/

├── Datasets/
│   ├── Income group.csv
│   ├── GDP_Current_USD.csv
│   ├── GDP_PC_Growth.csv
│   ├── Education.csv
│   ├── Military.csv
│   ├── Happiness.csv
│   ├── Prosperity.csv
│   └── Combined_Tableau_Analysis_2011_2021.csv
│
├── Final report DV.pdf
├── Global_Ankita_Tripathy.twbx
├── global-spending-prosperity-analysis.ipynb
├── requirements.txt
└── README.md

## License

This project is licensed under the MIT License. See the LICENSE file for details.
