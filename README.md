# Power BI Project : UPI Transactions Dashboard
# UPI Transactions Dashboard

This repository contains the Power BI project for analyzing UPI (Unified Payments Interface) transaction data. The dashboard provides comprehensive insights into transaction trends, financial distribution, and user behavior within the UPI ecosystem. It is designed to be an interactive tool for exploring key metrics and patterns, enabling data-driven decision-making.



## Features

The UPI Transactions Dashboard offers the following key features:

*   **Interactive Data Exploration**: Dynamic filtering capabilities across various dimensions such as bank names (sent/received), city, device type, gender, age, merchant account number, payment method, purpose, and transaction type.
*   **Monthly Transaction Analysis**: Visualizes the sum of transaction amounts by month, allowing for easy identification of trends and seasonal patterns in UPI transaction volumes.
*   **Remaining Balance Overview**: Provides a detailed breakdown of remaining balances by city and month, offering insights into financial distribution and activity across different urban centers.
*   **Comprehensive Data Set**: Built upon a rich dataset of 20,000 UPI transactions, ensuring robust analysis and accurate insights.
*   **User-Friendly Interface**: Designed for ease of use, enabling both data analysts and business users to quickly derive meaningful information.



## Data Source

The dashboard is powered by the `UPITransactionsDataset.xlsx` Excel file, which contains 20,000 entries of UPI transaction records. The dataset includes the following key columns:

| Column Name           | Data Type     | Description                                                               |
|:----------------------|:--------------|:--------------------------------------------------------------------------|
| `TransactionID`       | Object        | Unique identifier for each transaction.                                   |
| `TransactionDate`     | Datetime      | Date and time when the transaction occurred.                              |
| `Amount`              | Float         | The monetary value of the transaction.                                    |
| `BankNameSent`        | Object        | Name of the bank from which the transaction was initiated.                |
| `BankNameReceived`    | Object        | Name of the bank that received the transaction.                           |
| `RemainingBalance`    | Float         | The balance remaining after the transaction.                              |
| `City`                | Object        | City where the transaction took place.                                    |
| `Gender`              | Object        | Gender of the customer.                                                   |
| `TransactionType`     | Object        | Type of transaction (e.g., Transfer, Payment).                            |
| `Status`              | Object        | Status of the transaction (e.g., Success, Failed).                        |
| `TransactionTime`     | Object        | Time of the transaction.                                                  |
| `DeviceType`          | Object        | Type of device used for the transaction (e.g., Tablet, Laptop, Mobile).   |
| `PaymentMethod`       | Object        | Method used for payment (e.g., Phone Number, QR Code, UPI ID).          |
| `MerchantName`        | Object        | Name of the merchant involved in the transaction.                         |
| `Purpose`             | Object        | Purpose of the transaction (e.g., Food, Travel, Bill Payment, Shopping).  |
| `CustomerAge`         | Integer       | Age of the customer.                                                      |
| `PaymentMode`         | Object        | Mode of payment (e.g., Scheduled, Instant).                               |
| `Currency`            | Object        | Currency of the transaction (e.g., USD, EUR, GBP, INR).                   |
| `CustomerAccountNumber`| Integer       | Account number of the customer.                                           |
| `MerchantAccountNumber`| Integer       | Account number of the merchant.                                           |

This comprehensive dataset allows for multi-dimensional analysis, providing a holistic view of UPI transaction activities.



## Dashboard Visualizations

The Power BI project includes two main dashboard pages, each offering distinct views of the UPI transaction data:

### Dashboard 1: Transaction by Month

This dashboard features a column chart visualizing the sum of transaction amounts for each month in 2024. It provides a high-level overview of transaction volume trends throughout the year. The dashboard is equipped with various filters, including `BankNameSent`, `BankNameReceived`, `City`, `DeviceType`, `Gender`, `Age`, `MerchantAccountNumber`, `PaymentMethod`, `Purpose`, and `TransactionType`. These filters enable users to drill down into specific segments of the data, facilitating granular analysis of transaction patterns.

![Dashboard 1 - Transaction by Month](./UPI-Transactions-Dashboard/Dashboard1.png)

### Dashboard 2: Remaining Balance by City and Month

This dashboard presents a detailed table that breaks down the `RemainingBalance` by `City` and `Month`. It offers insights into the financial distribution and activity across different urban centers. Similar to Dashboard 1, this page also incorporates a comprehensive set of filters, allowing users to interactively explore remaining balance data based on specific criteria. This is particularly useful for identifying regional financial disparities or growth areas.

![Dashboard 2 - Remaining Balance](./UPI-Transactions-Dashboard/Dashboard2.png)



## How to Use

To interact with the UPI Transactions Dashboard, follow these steps:

1.  **Download Power BI Desktop**: If you don't already have it, download and install Power BI Desktop from the official Microsoft website.
2.  **Open the Project**: Open the `UPITransactionsAnalysis.pbix` file using Power BI Desktop.
3.  **Refresh Data (if necessary)**: Ensure the `UPITransactionsDataset.xlsx` file is in the same directory as the `.pbix` file, or update the data source settings within Power BI to point to its correct location. Then, refresh the data to load the latest information.
4.  **Explore Dashboards**: Navigate between "Page 1" (Transaction by Month) and "Page 2" (Remaining Balance by City and Month) to view different aspects of the data.
5.  **Apply Filters**: Utilize the various filter options at the top of each dashboard to slice and dice the data according to your analytical needs. You can filter by bank, city, device type, gender, age, and more.
6.  **Analyze Insights**: Observe the charts and tables to identify trends, patterns, and anomalies in UPI transaction data. Use the interactive features to gain deeper insights into specific segments.


