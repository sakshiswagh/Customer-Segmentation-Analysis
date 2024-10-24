# Customer-Segmentation-Analysis

Data Cleaning and Analysis Project
This project involves cleaning and preparing customer, product, region, and transaction datasets for analysis and reporting in Power BI. Below is a detailed explanation of the cleaning steps taken for each dataset.

1. Customer Dataset Cleaning Process
Columns: CustomerID, Email, Phone, City, State, Country, Gender, Age, JoinedDate, LastPurchaseDate, TotalSpent, LoyaltyPoints, PurchaseFrequency, CustomerSegment, PreferredPaymentMethod, MaritalStatus, AccountCreationDate, AccountStatus, LastUpdated, ReferrerID, FeedbackRating, EmailDomain, CountryCode

Cleaning Steps:
Data Import: Imported the dataset into Power BI via Get Data > Text/CSV.
Remove Invalid Email Domains: Cleaned the Email column by removing invalid or incorrectly formatted email domains.
Standardize Phone Numbers: Reformatted phone numbers to ensure consistency across records (e.g., +91-98765-43210).
Handle Missing Values: Replaced or imputed missing values logically in important columns like AccountStatus, MaritalStatus, and FeedbackRating.
Correct Data Types: Ensured each column has the appropriate data type (e.g., Date for JoinedDate, Number for TotalSpent).
Extract Email Domains: Added a derived column (EmailDomain) to capture the domain part of email addresses.
Customer Segmentation: Created new classifications for customers based on TotalSpent and LoyaltyPoints.
Standardize Dates: Applied uniform date formatting across all date columns.
Standardize Country Codes: Ensured that country codes are properly formatted, including adding the correct prefix (e.g., +1 for US).
2. Product Dataset Cleaning Process
Columns: ProductID, ProductName, Category, Price, StockStatus, Supplier, UpdatedPrice, UpdatedStockStatus, LastUpdated, Discontinued

Cleaning Steps:
Remove Duplicates: Ensured that each ProductID is unique and removed duplicate entries.
Handle Missing Values: Filled missing values for Price and StockStatus using appropriate methods.
Price Standardization: Ensured consistency in price formatting (e.g., ₹500.00).
Data Types: Standardized column types, ensuring Price is numerical and ProductName is text.
Discontinued Products: Updated the Discontinued column where necessary to accurately reflect the product status.
3. Region Dataset Cleaning Process
Columns: RegionID, RegionName, Country, State, UpdatedRegionName, LastUpdated, CountryCode

Cleaning Steps:
Filter Invalid Regions: Removed entries with invalid or incomplete RegionName values.
Standardize Country Codes: Ensured all country codes follow the same format (e.g., +91 for India).
Handle Missing Data: Used logical imputation or filled down missing region data.
Correct Data Types: Ensured that RegionName is text and CountryCode is numerical.
4. Transaction Dataset Cleaning Process
Columns: TransactionID, CustomerID, ProductID, TransactionDate, Quantity, TotalAmount, PaymentMethod, DiscountApplied, LastUpdated

Cleaning Steps:
Remove Duplicates: Ensured TransactionID is unique by removing any duplicate transactions.
Handle Missing Values: Imputed missing values in critical columns like Quantity and TotalAmount.
Correct Data Types: Made sure that TransactionDate is in date format and TotalAmount is numeric.
Standardize Payment Methods: Created uniform labels for different payment methods (e.g., Credit Card, PayPal).
Validate Discounts: Ensured DiscountApplied is properly recorded and consistent.
Conclusion
All datasets have been cleaned and prepared for analysis. Each dataset now contains structured, consistent, and error-free data, ready for visualization in Power BI and further reporting.
