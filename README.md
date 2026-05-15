# Analysis of Credit Card Expenditures and Payments with Forecast via SQL and Tableau

A client concerned about credit card debt requested an analysis of spending and payments, along with a forecast of future expenses.

## Technologies and Tools
1. Data was imported into **PostgreSQL** database (version 17.9) which resides in the cloud hosted by aiven (https://console.aiven.io/).
2. Performed cleaning and analysis with **Beekeeper Studio** (https://www.beekeeperstudio.io/db/postgres-client/) and **PgAdmin 4** (https://www.pgadmin.org/) SQL clients.
3. Created visualizations with **Tableau** (version 2026.1. professional edition ).
4. Detailed notes and code snippets presented in **Google Colab**.

## Questions at project outset (determined by developer/client consultation)
1. How is the client keeping up with expenses?
1. Where is the money going?  When is it going there?
3. Are there categories, vendors, or certain time periods to concentrate on for reducing expenses?
5. Are there a meaningful correlations in the data?
6. What are the suggestions for the future?
7. What is the forecast for future expenditures taking suggestions into account?

## Process
1. Client provide extracts from two credit cards as .csv files.
2. Import files into postgres using PgAdmin 4 import/export tool.
3. Merged the two sources into a single table and normalized data (i.e. categories) in SQL.
4. Cleaned the data added vendor column via extract from description column with SQL.
5. Created a view on top of the two merged tables for analysis in tableau.
6. Performed exploratory data analysis and incorporated into dashboards using tableau.
7. Created a future forecast of expenditures using SQL and created visualization in tableau.  
*_detailed notes and data definitions within google colab notebook_

## Limitations
1. Data provided was only for eleven months.  This totaled 941 records, which is a small amount limiting the ability to find seasonal trends and cycles resulting in difficulty creating a detailed forecast for the future.

