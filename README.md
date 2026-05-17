# Analysis of Credit Card Expenditures and Payments with Forecast via SQL and Tableau

A client concerned about credit card debt requested an analysis of spending and payments, along with a forecast of future expenses. 

[Published Viz for Project](https://public.tableau.com/app/profile/mark.meschi/viz/Credit_Card_Spending_Analysis/Home)

## Technologies and Tools
1. Data was imported into **PostgreSQL** database (version 17.9) which resides in the cloud hosted by [**aiven**](https://console.aiven.io/).
2. Performed cleaning and analysis with [**Beekeeper Studio**](https://www.beekeeperstudio.io/db/postgres-client/)[^1]  (version 5.72) and [**PgAdmin 4**](https://www.pgadmin.org/) (version 9.14) SQL clients.
3. Created visualizations with [**Tableau Public Edition**](https://www.tableau.com/products/public) (version 2026.1.26.0410.0924).
4. Detailed notes and SQL code snippets presented in [**Google Colab**](https://colab.research.google.com/)[^2].
5. SQL code formatted using [**SQLFormat**](https://sqlformat.org/).
6. README.txt markdown created with [**Typora**](https://typora.io/) (version 1.13.4).

## Questions at project outset (determined by developer/client consultation)
1. How is the client keeping up with expenses?
1. Where is the money going?  When is it going there?
3. Are there categories, vendors, or certain time periods to concentrate on for reducing expenses?
5. Are there a meaningful correlations in the data?
6. What are the suggestions for the future?
7. What is the forecast for future expenditures taking suggestions into account?

## Process[^3]
1. Client provided extracts from two credit cards as .csv files.
2. Import files into postgres using PgAdmin 4 import/export tool.
3. Merged the two sources into a single table and normalized data (i.e. categories) in SQL.
4. Cleaned the data added vendor column via extract from description column with SQL.
5. Created a view on top of the two merged tables for analysis in tableau.
6. Performed exploratory data analysis and incorporated into dashboards using tableau.
7. Created a future forecast of expenditures using SQL and created visualization in tableau. 


## Limitations and Notes
1. Data provided was only for eleven months.  This totaled 941 records, which is a small amount limiting the ability to find seasonal trends and cycles resulting in difficulty creating a detailed forecast for the future.
2. Google colab notebook can be opened by going to their website [Google Colab](colab.research.google.com) then going to File->Open Notebook->GitHub then entering in the URL for this project (https://github.com/mdmeschi72/CreditCardSpendingAnalysis).

[^1]: **LOVE** Beekeeper Studio because it allows you to toggle to vim as its editor.
[^2]: Google colab has database password embedded in _secrets_ for security reasons.
[^3]: Detailed notes and data definitions within google colab notebook.

