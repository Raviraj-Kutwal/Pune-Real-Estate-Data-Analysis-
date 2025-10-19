Pune RERA Real Estate Analysis

📖 About The Project

This project performs an in-depth analysis of the Pune real estate market using a dataset of projects registered under the Real Estate Regulatory Authority (RERA). The analysis covers data cleaning, preprocessing, and visualization to uncover key insights into project statuses, leading promoters, property types, and sales distribution across different divisions of Pune.

🛠️ Tools Used

The analysis was conducted using Python with the following core libraries:

Pandas: For data manipulation and analysis.

NumPy: For numerical operations and handling missing values.

Matplotlib & Seaborn: For data visualization and generating insightful plots.

🔄 Data Preprocessing

To ensure the accuracy and reliability of the insights, the raw dataset underwent several preprocessing steps:

Loading Data: The primary dataset pune-rera-dataset.csv and a supplementary pincode.csv were loaded into Pandas DataFrames.

Handling Duplicates: The dataset was checked for duplicate project entries based on the rera id , several thousands of duplicates were found and handled.

Column Removal: Irrelevant columns that were not required for the analysis, such as location_lat_long, number_of_basements, and number_of_podiums, etc were dropped to simplify the dataset.

Missing Value Imputation:

Empty strings and various text representations of null values (e.g., 'none', 'null', 'na') were standardized to np.nan.

A significant number of missing values were identified in columns like revised_proposed_date_of_completion, extended_date_of_completion, cases_count, and complaints_count.

Data Enrichment: The RERA dataset was merged with the pincode.csv dataset on the pincode to add geographical information, including DivisionName, OfficeName, and RegionName.

Duplicate Resolution after Merge: The merge operation introduced duplicates for projects located in areas with multiple office names for a single pincode. These duplicates were resolved by keeping only the first entry for each unique rera_id.

📊 Key Insights Generated

Promoter Market Share

The analysis identified the top real estate promoters in Pune based on the number of registered projects.

Top 15 Promoters by Number of Projects:

1.  **Joyville Shapoorji Housing Private Limited** (35 projects)
2.  **Macrotech Developers Limited** (34 projects)
3.  **Lavasa Corporation Ltd** (31 projects)
4.  **PANDIT JAVDEKAR ASSOCIATES** (28 projects)
5.  **PARANJAPE SCHEMES (CONSTRUCTION) LTD** (24 projects)
6.  **VTP REALTY LLP** (24 projects)
7.  **KOLTE PATIL DEVELOPERS LTD** (23 projects)
8.  **MAHALAXMI BUILDCON** (23 projects)
9.  **GODREJ PROPERTIES LIMITED** (22 projects)
10. **Goel Ganga Developments** (20 projects)
11. **VILAS JAVDEKAR DEVELOPERS PRIVATE LIMITED** (19 projects)
12. **PRIDE AND EXPERT PROPERTIES LLP** (18 projects)
13. **Shapoorji Pallonji And Company Private Limited** (18 projects)
14. **AMANORA PARK TOWN** (18 projects)
15. **Gagan Developers** (17 projects)

Project Status Distribution

A significant majority of the projects in the dataset are ongoing, indicating a continuously active real estate market in Pune.

Project Area by Property Type

Residential projects dominate the Pune real estate market in terms of total area, followed by 'Others' and 'Plots'.

Sales Analysis by Division

The analysis of booked apartments and plots reveals the sales activity across different administrative divisions of Pune. The Pune City East Division shows the highest number of booked apartments.

Booked Apartments by Division:

Booked Plots by Division:

The total number of booked properties (apartments + plots) across all projects with sales is 525,022.

This analysis provides a comprehensive overview of the Pune RERA registered properties, offering valuable insights for potential homebuyers, investors, and real estate developers.
---

## 🗂️ Data Sources

- **MahaRERA Official Portal:** [https://maharera.mahaonline.gov.in](https://maharera.mahaonline.gov.in)  
- **India Post / Data.gov.in:** National Postal PIN Code Database  

