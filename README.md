
# 📊 Facebook Ad Campaign Performance Analysis

This project explores and analyzes a Facebook ad campaign dataset to uncover key insights that drive marketing decisions. The dataset includes impressions, clicks, conversions, and demographic attributes like age and gender.

---

## 🧹 Data Cleaning

The original dataset had a formatting issue starting from **row 763**, where:

- Values were shifted **two columns to the left**, resulting in incorrect data alignment.
- Columns `campaign_id` and `fb_campaign_id` were overwritten.

### Fix:
To resolve this, I manually cleaned the dataset using Excel by:
- Keeping columns A, B, and C (`ad_id`, `reporting_start`, `reporting_end`) unchanged.
- Shifting values in columns D and onward **two columns to the right** for affected rows.
- Leaving `campaign_id` and `fb_campaign_id` as null in those rows.

The cleaned dataset is saved as:

```
cleaned_facebook_ads.csv
```

---

## 📈 KPIs Calculated

Using Python, I calculated the following key metrics:
- **CTR (Click-Through Rate)** = Clicks / Impressions
- **CPC (Cost Per Click)** = Spend / Clicks
- **CPA (Cost Per Approved Conversion)** = Spend / Approved Conversions

---

## 📊 Power BI Dashboard (Coming Soon)

A Power BI dashboard is under development to visualize:
- Performance by Age Group and Gender
- Top-performing Campaigns
- Cost Efficiency Metrics

---

## 🛠️ Tech Stack

- Python (Pandas, Matplotlib)
- Power BI
- Excel (for quick data correction)
- VS Code

---

## 📁 Dataset

[Facebook Ad Campaign Dataset on Kaggle](https://www.kaggle.com/datasets/madislemsalu/facebook-ad-campaign)
