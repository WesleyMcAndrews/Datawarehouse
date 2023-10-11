# Surgical Prosthetics Data Warehouse Project

This repository is part of a data warehousing project created by a Data Scientist for a surgical prosthetics reselling company. The project is built using Microsoft SQL Server Integration Services (SSIS) for Extract, Transform, Load (ETL) processes, Microsoft SQL Server for the database, and Microsoft SQL Server Analysis Services (SSAS) for Online Analytical Processing (OLAP) and data mining. The data warehouse consists of multiple datamarts, including Inventory, Purchases, Sales, and Financials.

## Data Warehouse Structure

A data warehouse is structured with a central repository for data, comprising fact tables, dimension tables, and decision cubes. 

- **Fact Table**: The fact table is the core of the data warehouse, containing quantitative data (measures) that represent the business transactions. It records key performance indicators (KPIs) and serves as the foundation for creating reports and analyzing data. In this project, the fact table includes data related to the core business activities of the prosthetics reselling company, such as inventory levels, purchase transactions, sales transactions, and financial data.

- **Dimension Tables**: Dimension tables store descriptive data that provide context to the measures in the fact table. Dimensions act as the primary entry points for querying the data warehouse. In this project, dimension tables include information about products, suppliers, manufacturers, invoices, customers, and time.

- **Decision Cubes**: Decision cubes are used in OLAP systems to facilitate multidimensional analysis. They are constructed from fact and dimension tables and allow users to explore data from different perspectives. Cubes simplify the process of drilling down or rolling up data to gain insights. In this project, multiple cubes are created for each datamart, enabling business users to analyze data related to inventory, purchases, sales, and financials.

## Datamarts

This data warehouse project comprises four datamarts, each designed to serve a specific business function:

### Inventory Datamart

- **Dimensions**:
  - Product: Information about the prosthetic products in stock.
  - Entries: Details of inventory entries, including quantities, dates, and sources.
  - Exits: Information on inventory exits, including quantities, dates, and destinations.
  - Time: Temporal information for time-based analysis.

### Purchases Datamart

- **Dimensions**:
  - Products: Details of the products purchased.
  - Suppliers: Information about the suppliers providing the prosthetic products.
  - Manufacturers: Data related to the manufacturers of the products.
  - Purchases: Transaction data, including quantities and dates.
  - Time: Temporal information for time-based analysis.

### Sales Datamart

- **Dimensions**:
  - Invoices: Invoice data, including invoice numbers, dates, and payment terms.
  - Contracts: Information about contracts or agreements with customers.
  - Hospitals: Details of the hospitals or medical institutions where sales occur.
  - Salespersons: Data on the salespeople handling the transactions.
  - Sales: Transaction data, including quantities and prices.
  - Products: Details of the products sold.
  - Manufacturers: Information about product manufacturers.
  - Time: Temporal information for time-based analysis.

### Financial Datamart

- **Dimensions**:
  - Sales: Sales data, including quantities, prices, and totals.
  - Invoices: Invoice data, including invoice numbers, dates, and payment terms.
  - Products: Product-specific financial information.
  - Customers: Information about the customers.
  - Invoices: Invoice data, including invoice numbers, dates, and payment terms.
  - Payments: Data related to payments received.
  - Time: Temporal information for time-based analysis.

## Technologies Used

- **ETL**: Microsoft SQL Server Integration Services (SSIS)
- **Database**: Microsoft SQL Server
- **OLAP and Data Mining**: Microsoft SQL Server Analysis Services (SSAS)

## Conclusion

This data warehousing project serves as a powerful tool for the surgical prosthetics reselling company to gain valuable insights into their inventory, purchasing, sales, and financial data. By structuring data into fact tables, dimension tables, and decision cubes, this data warehouse enables in-depth analysis, reporting, and decision-making to optimize business operations and performance.

For more information and to explore the code and design of this data warehouse project, please refer to the respective folders and files in this repository.
