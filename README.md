# Quantium_Data_Analytics

# Project Background

Quantium is an Australian-based data science and artificial intelligence company founded in 2002, specializing in advanced analytics solutions that drive strategic decision-making for businesses.

The company delivers data-driven insights across industries such as retail, finance, healthcare, and FMCG, leveraging transactional, behavioral, and demographic data to optimize business performance.

This project focuses on retail analytics, specifically analyzing *customer purchasing behavior within the chips category for a supermarket client.* The goal is to extract actionable insights to improve category performance and inform strategic planning. 

The analysis includes:
- **Data Cleaning & Preparation**: Handling of missing values, filtering of relevant product categories, and standardization of transaction records.
- **Customer Segmentation**: Identification of key customer groups based on purchasing frequency and product preferences.
- **Sales Performance**: Analysis of total sales, average transaction values, and key sales drivers.
- **Product Insights**: Examination of chip brand preferences, packet size impact, and purchasing trends.
- **Strategic Recommendations**: Development of data-driven recommendations for category optimization and customer targeting.


The Pandas library utilized to inspect and perform quality checks can be found [here](./notebooks/Quantium_data_checks.ipynb).

The Pandas library utilized to organize, prepare and merge data can be found [here](./notebooks/Qiuantium_data_transformation.ipynb).

Targeted pandas code regarding various business questions can be found [here](./notebooks/Quantium_business_analysis.ipynb).



# Data Structure & Initial Checks

Quantium’s dataset consists from two files purchase_behaviour.csv (72,637 records) and transaction_data.xlsx (246,835 records).

<img width="721" alt="ERD" src="https://github.com/user-attachments/assets/2c68e9dd-5c90-4951-be47-620ce0fab848" />


Prior to beginning the analysis, a variety of checks were conducted for quality control and familiarization with the datasets. The Pandas library utilized to inspect and perform quality checks can be found here.

# Executive Summary

### Overview of Findings

The analysis of 2018–2019 sales data highlights key trends in customer preferences, product sales, and brand performance. Older Families make up the largest share of Budget sales, while Young Singles/Couples drive Mainstream purchases. 175g packs are the top-selling size, generating the highest revenue. Among brands, KETTLE leads in both sales and revenue, followed by DORITOS and SMITHS. The following sections explore these insights in more detail, with key metrics and trends, and highlight key opportunity areas for improvement.

![ProportionOfSales](https://github.com/user-attachments/assets/aa1ce97b-eb08-4230-82fa-5b3318d2b3c0)

The complete set of analysis plots is available for download [here](./plots).


### **Customer segment sales and proportions**

1. **Older Families** drive the highest **Budget sales (47.7%)**, meaning they are price-sensitive but a **consistent revenue driver.**
2. **Young Singles/Couples** have the highest **Mainstream share** and contribute even more to Mainstream sales (60.5%).
3. **Midage Singles/Couples** account for **33.2% of Premium customers**, aligning with their notable **31.6% Premium sales share.**
4. **New Families & Older Families** have lower **Premium sales contribution (<25%)**, suggesting they either **purchase less frequently or in smaller quantities.**

![proportionOfCustomers](https://github.com/user-attachments/assets/de92d59d-a393-4e5d-9c77-0c23d2b1e279)


### **Packet Size Analysis: Sales, Revenue, and Pricing Trends**

**Sales Volume by Packet Size** 

- The **175g packet size** has the **highest sales volume**, with **around 120,000 units sold,** meaning it has the **highest purchase frequency**.
- The **150g packet size** is the **second best-selling** size, with up to **80,000 units sold**.
- The **110g, 134g, 165g, and 170g** packet sizes are also among the **most popular**, each selling more than **20,000 units**.

![salesVolumeByPacketSize](https://github.com/user-attachments/assets/d37d0f09-e5a7-43aa-b5bb-1f6a43d5701a)


**Revenue Contribution by Packet Size** 

- The **175g packet size generates the highest revenue**, contributing almost **$500,000**.
- **150g packets** also have **strong revenue performance**, bringing up to **$300,000.**

![RevenueContributionByPacketSize](https://github.com/user-attachments/assets/7a3e36d3-f67f-419a-aa0a-2d00458e11a9)

**Price per Gram by Packet Size** 

- Smaller packets **(≤125g)** have the **highest price per gram**, averaging **$0.02–$0.035 per gram**.
- **The 175g and 150g** packet sizes have **moderate price - $0.023 - $0.025 per gram**.
- Larger packets **(≥200g) have the lowest price per gram**, around **$0.018 per gram**.
- **Smaller packs are priced at a premium**, while **larger packs offer cost savings per gram**, likely encouraging bulk purchases.

![pricePerGramByPacketSize](https://github.com/user-attachments/assets/4c2910d5-dd2a-416a-9221-d49164906aec)

### Brand loyalty

- **KETTLE** is the **top-performing brand**, generating **21,6% of total revenue** and selling **16,8% of total units.**
- **DORITOS** ranks **second in revenue** with **12,5%**, but its sales volume (**10,3%**) is lower than SMITHS (**12,2%**).
- **PRINGLES** and **INFUZIONS** have **lower sales volumes (10,2% & 5,8%** of total ****units sold respectively**),** but **PRINGLES** maintains a **stronger revenue** position **(9,8%).**

![totalQuantitySoldByBrand](https://github.com/user-attachments/assets/e8ca7548-ad16-462e-9546-133cd05ba55a)

![totalRevenueByBrand](https://github.com/user-attachments/assets/6566ccc6-38fd-46d6-937c-b9f80722f568)

### Recommendations:

Based on the uncovered insights, the following recommendations have been provided:

- Older Families contribute **47.7%** of budget sales, indicating they are consistent and reliable revenue drivers. These families are **highly price-sensitive**, which makes them an ideal target for promotions focused on **bulk purchases** and **larger pack sizes**.
- Young Singles and Couples drive **60.5%** of mainstream sales, making them a major contributor to overall sales. Their purchasing behavior suggests they are likely to purchase **mid-sized packs**, particularly the **175g** and **150g** options, generating significant revenue ($500,000 and $300,000, respectively).
- Mid-Age Singles/Couples represent **33.2%** of premium sales. To target them, introduce **exclusive premium bundles** or loyalty programs that emphasize high-quality chips in the **175g** or **150g** packets. The **PRINGLES** brand, in particular, accounts for **9.8%** of total revenue, demonstrating strong performance within this segment.
- New Families, along with Older Families, contribute less to **premium sales** (<25%), suggesting a preference for value over premium pricing. However, they are likely to engage with **larger pack sizes**, which offer better value per gram, especially the **200g** or larger packets. The **200g** packets are priced at **$0.018 per gram**, making them an attractive option for price-sensitive buyers.
- **KETTLE** is responsible for **21.6%** of total revenue, and **PRINGLES** accounts for **9.8%**. Promote **KETTLE** and **PRINGLES** more prominently in high-traffic areas and online platforms. Given their solid revenue contribution, a strategic push in these locations could further enhance their visibility and sales.
