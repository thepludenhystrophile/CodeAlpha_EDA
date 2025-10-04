# CodeAlpha_EDA
Exploratory Data Analysis on Drug Reviews dataset

## 💊 Project Overview
This project performs Exploratory Data Analysis (EDA) on the Drug Review Dataset to uncover patterns, trends, and insights about patient experiences with different drugs and conditions. The goal is to prepare a clean dataset and extract actionable findings before applying further analysis techniques.

## 📂 Dataset Description

• Training dataset: 161,297 entries, 7 columns

• Testing dataset: 53,766 entries, same structure

• Unique drugs: 34,336

• Unique conditions: 885

• File saved after cleaning: drugreviews_clean.csv

## 🛠️ Data Cleaning

• Handled 899 missing values in the condition column → replaced with "Unknown".

• No duplicate rows found.

• Standardized ratings to be within 1–10.

• Standardized date formats and corrected inconsistences.

## 🔑 Key Insights

### 1. Dataset Structure
• Large dataset with wide diversity in drugs and therapeutic areas.

• Condition column standardized → "Unknown" for missing cases.

### 2. Ratings Distribution
• Ratings are positively skewed (median = 8, max = 10).

• Most reviews are either very positive (10/10) or very negative (1/10).

• Neutral/mid-range ratings are rare.

• Sentiment mapping (rating → sentiment):
• ~60% Positive
• ~25% Negative
• ~15% Neutral

➝ ⚠️ Indicates class imbalance — important for future modeling.

### 3. Top Drugs & Conditions
• Most reviewed drugs: Levonorgestrel, Etonogestrel, Estradiol-based.

• Most common conditions: Birth Control (~28k), Depression, Pain, Anxiety, Acne.

• Levonorgestrel alone: ~36k reviews.

### 4. Trends Over Time
• Review volume increased sharply after 2014, peaked in 2016–2017, then declined.

• Average ratings decreased over time, showing a trend toward more critical reviews.

### 5. Condition-Specific Findings
• Birth Control: Most reviewed (~28k), but lower mean rating (~6.1), showing mixed experiences.

• Depression, Pain, Anxiety, Acne: Higher median ratings (8–9).

• Statistical tests:
• Kruskal–Wallis (p < 0.001) → significant differences.

• Post-hoc Tukey HSD → Birth Control rated significantly lower.

### 6. Drug-Specific Findings
• Phentermine, Sertraline, Levonorgestrel → Highest user ratings (median ~9–10).

• Ethinyl estradiol–based drugs → Lower ratings (median ~6), more variability.

• Differences statistically significant (Kruskal–Wallis p < 0.001).

### 7. Review Characteristics
• Median review length: ~100 words.

• Outliers: Some > 1,000 words (e.g., Venlafaxine, Prozac, Copper IUD).

• Weak positive correlation (r ≈ 0.23) between rating and usefulness votes.

## 📊 Key Visualizations
• Distribution of Ratings (Histogram)
![Rating distribution](data/visuals/rating_distribution.png)

• Top 10 Conditions by Review Count (Bar Chart)

• Rating Trends Over Time (Line Chart)

• Boxplots comparing Ratings across Top Drugs/Conditions

Full visualizations are available in the [visuals folder](data/visuals/)

## Conclusion
The dataset shows strongly polarized patient experiences — reviews are either highly positive or highly negative, with few neutral cases. Hormonal drugs (especially birth control–related) dominate the dataset but receive mixed or lower ratings compared to psychiatric drugs (e.g., Sertraline, Phentermine). The temporal trend highlights increasing review activity until 2017, followed by declining volumes and slightly lower ratings.

These findings provide a clean foundation for future sentiment analysis, predictive modeling, or healthcare business intelligence applications.

## 📮 Contact

**Elizabeth Ayeku** 
- Email: temiloluwaayeku@gmail.com 
