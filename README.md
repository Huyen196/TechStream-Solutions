# TechStream Solutions
The company is called "TechStream Solutions", and the product is a Software as a Service (SaaS) platform named "Streamline Pro". This platform provides comprehensive project management and collaboration tools for businesses of all sizes.

TechStream Solutions has been operating for several years and has gathered significant data on their costs and revenues. They are now looking to analyze their unit economics to understand the profitability of Streamline Pro on a per-customer basis.

By performing these calculations, TechStream Solutions aims to:

- Identify the profitability of acquiring and retaining customers.
- Assess the efficiency of their marketing and sales strategies.
- Make informed decisions on scaling their operations and optimizing their resource allocation.
- This information will guide TechStream Solutions in refining their business strategies, ensuring sustainable growth, and maximizing profitability.

## Import data

All raw data were collected and formatted by excel. There are 5 datasets as below:

1. Customer Lifespan
   
|    |   Unnamed: 0 | start_date          | churn_date          |   lifespan_days |
|---:|-------------:|:--------------------|:--------------------|----------------:|
|  0 |         1000 | 2021-11-15 00:00:00 | 2022-09-14 00:00:00 |             303 |
|  1 |         1001 | 2022-04-15 00:00:00 | 2023-02-16 00:00:00 |             307 |
|  2 |         1002 | 2022-10-30 00:00:00 | 2023-02-04 00:00:00 |              97 |
|  3 |         1003 | 2021-08-22 00:00:00 | 2023-02-07 00:00:00 |             534 |
|  4 |         1004 | 2021-08-23 00:00:00 | 2022-02-02 00:00:00 |             163 |

2. Daily marketing spending

|    | date                | channel      |   spending |
|---:|:--------------------|:-------------|-----------:|
|  0 | 2023-01-01 00:00:00 | Google Ads   |        784 |
|  1 | 2023-01-01 00:00:00 | Facebook Ads |        659 |
|  2 | 2023-01-01 00:00:00 | LinkedIn Ads |        729 |
|  3 | 2023-01-01 00:00:00 | Twitter Ads  |        292 |
|  4 | 2023-01-02 00:00:00 | Google Ads   |        935 |

3. Monthly expense

|    |   # | month               | category          | item                 |   amount |
|---:|----:|:--------------------|:------------------|:---------------------|---------:|
|  0 |   1 | 2023-01-01 00:00:00 | Server Costs      | AWS Hosting          |     8000 |
|  1 |   2 | 2023-01-01 00:00:00 | Server Costs      | Google Cloud Storage |     4000 |
|  2 |   3 | 2023-01-01 00:00:00 | Software Licenses | Atlassian Jira       |     1200 |
|  3 |   4 | 2023-01-01 00:00:00 | Software Licenses | Slack                |      800 |
|  4 |   5 | 2023-01-01 00:00:00 | Software Licenses | Salesforce           |     1500 |

4. Payroll

|    | month               | department   | employee_name   | position          |   paid | yyyy-mm   |
|---:|:--------------------|:-------------|:----------------|:------------------|-------:|:----------|
|  0 | 2023-01-01 00:00:00 | Sales        | John Doe        | Sales Manager     |   1500 | 2023-01   |
|  1 | 2023-01-01 00:00:00 | Sales        | Jane Smith      | Sales Associate   |    600 | 2023-01   |
|  2 | 2023-01-01 00:00:00 | Sales        | Jim Brown       | Sales Associate   |    700 | 2023-01   |
|  3 | 2023-01-01 00:00:00 | Sales        | Laura Miller    | Sales Associate   |    800 | 2023-01   |
|  4 | 2023-01-01 00:00:00 | Marketing    | Alice Johnson   | Marketing Manager |   1650 | 2023-01   |

5. Receipts history

|    | date                |   customer_id |   receipt_amount |   new_customer |
|---:|:--------------------|--------------:|-----------------:|---------------:|
|  0 | 2023-01-01 00:00:00 |          2653 |               67 |              1 |
|  1 | 2023-01-01 00:00:00 |          2731 |              271 |              1 |
|  2 | 2023-01-01 00:00:00 |          1277 |              231 |              0 |
|  3 | 2023-01-01 00:00:00 |          2094 |              107 |              0 |
|  4 | 2023-01-01 00:00:00 |          1314 |              416 |              0 |

## Caculation

1. Customer Acquisition cost (CAC)


