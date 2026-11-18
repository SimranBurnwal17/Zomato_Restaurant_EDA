# 🍽️ Zomato Restaurant Data Analysis | Exploratory Data Analysis (EDA)

## 📌 Project Overview

This project focuses on performing Exploratory Data Analysis (EDA) on a Zomato restaurant dataset containing **9,551 restaurants across multiple countries**.

The objective is to explore restaurant ratings, cuisines, pricing, customer engagement, and online delivery services to identify meaningful patterns and business opportunities.

Using Python and its data analysis and visualization libraries, this project transforms raw restaurant data into actionable insights that can support business decision-making.

## 🎯 Business Objectives

- Identify cities with the highest number of restaurants.
- Analyze restaurant ratings and their distribution.
- Understand the relationship between restaurant ratings, votes, and pricing.
- Explore the most popular and highest-rated cuisines.
- Evaluate the relationship between online delivery and restaurant ratings.
- Analyze customer engagement through restaurant votes.
- Identify missing values, duplicates, and outliers.
- Generate business recommendations based on the analysis.

## 🛠️ Tools & Technologies

| Technology | Purpose |
|---|---|
| Python | Programming and data analysis |
| Pandas | Data cleaning and manipulation |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Jupyter Notebook | Interactive data analysis |

## 🔄 Project Workflow

### 1. Data Loading and Understanding

- Imported the dataset using Pandas.
- Explored the first few records.
- Examined dataset dimensions and column names.
- Analyzed data types and statistical summaries.
- Identified numerical and categorical variables.

### 2. Data Quality Assessment and Cleaning

- Identified missing values across columns.
- Checked for duplicate records.
- Handled missing values in the Cuisines column by replacing them with "Unknown".
- Examined inconsistent values in Yes/No categorical columns.
- Evaluated overall data completeness.

### 3. Univariate Analysis

Analyzed individual variables to understand their distributions.

- Distribution of restaurant ratings.
- Frequency of rating categories.
- Distribution of restaurant price ranges.
- Distribution of restaurant votes.
- Top cities by restaurant count.

### 4. Bivariate Analysis

Explored relationships between two variables.

- Restaurant ratings vs. votes.
- Restaurant ratings vs. price range.
- Table booking vs. online delivery.
- Restaurant ratings vs. online delivery availability.
- Average ratings across different price categories.

### 5. Multivariate Analysis

Explored relationships among multiple variables.

- Correlation analysis of numerical variables.
- Pair plot analysis.
- Average ratings by city and online delivery availability.
- Price range and online delivery comparisons.

### 6. Outlier Analysis

Identified potential outliers using:

- Interquartile Range (IQR) method.
- Z-Score method.
- Box plots for Votes, Average Cost for Two, and Aggregate Rating.

Outliers were evaluated in their business context rather than automatically removed, since unusually high votes or costs may represent genuine restaurant performance.

### 7. Feature Transformation and Dataset Preparation

- Converted Yes/No values into binary 1/0 values for selected columns.
- Created an `Is Rated` feature to distinguish rated restaurants from unrated restaurants.
- Generated a cleaned dataset containing 22 columns.
- Exported the processed dataset as `zomato_clean.csv`.

## 📊 Key Findings and Business Insights

### 1. Restaurant Market Concentration

New Delhi has the highest restaurant count, with 5,473 restaurants, followed by Gurgaon (1,118) and Noida (1,080).

Together, these three cities account for approximately 80.3% of the restaurants in the dataset.

**Business Implication:** Zomato could explore expansion opportunities in less represented cities while continuing to strengthen its presence in major markets.

### 2. Customer Rating Distribution

Out of 9,551 restaurants, 2,148 are classified as "Not rated", representing approximately 22.49% of the dataset.

**Business Implication:** Encouraging customers to submit restaurant reviews could improve rating coverage and provide more information for restaurant discovery.

### 3. Restaurant Pricing and Ratings

The average ratings across different price ranges are:

| Price Range | Average Rating |
|---|---:|
| 1 – Cheap | 3.24 |
| 2 – Moderate | 3.38 |
| 3 – Expensive | 3.78 |
| 4 – Very Expensive | 3.89 |

**Business Implication:** Higher-priced restaurants have higher average ratings in this dataset. However, price alone should not be treated as the reason for better ratings.

### 4. Online Delivery and Table Booking

The analysis shows:

- Approximately 25.7% of restaurants offer online delivery.
- Approximately 12.1% of restaurants offer table booking.

**Business Implication:** There may be opportunities to expand these services among restaurants that currently do not offer them.

### 5. Factors Associated with Restaurant Ratings

The correlation analysis shows:

| Variable | Correlation with Aggregate Rating |
|---|---:|
| Price Range | 0.438 |
| Votes | 0.314 |
| Average Cost for Two | 0.052 |

**Business Implication:** Price range and votes show positive associations with restaurant ratings, while average cost for two has a very weak linear relationship. Correlation does not establish causation.

## 💡 Business Recommendations

Based on the analysis, the following opportunities can be explored:

1. **Improve Rating Coverage:** Encourage customers to submit ratings for restaurants currently classified as Not Rated.
2. **Expand Online Delivery:** Explore opportunities to onboard more restaurants onto the online delivery platform.
3. **Promote Table Booking:** Investigate opportunities to increase table booking adoption.
4. **Explore New Markets:** Identify growth opportunities in cities with relatively low restaurant representation.
5. **Improve Restaurant Visibility:** Encourage new restaurants to build customer engagement and collect reviews.

## 📁 Repository Structure

```text
zomato-restaurant-eda/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   └── Zomato_EDA_Analysis.ipynb
│
├── reports/
│   └── business_insights.md
│
├── requirements.txt
├── .gitignore
└── README.md
```

## 📂 Dataset Information

The project uses a Zomato restaurant dataset containing 9,551 restaurant records and 21 original columns.

The cleaned dataset contains 22 columns after feature transformation.

The original and processed CSV files are hosted externally due to their file sizes.

**Dataset Download:** [Access the dataset on Google Drive](PASTE_YOUR_GOOGLE_DRIVE_LINK_HERE)

### Dataset Files

- `zomato.csv` – Original restaurant dataset.
- `zomato_clean.csv` – Cleaned and processed dataset.

## 🚀 How to Run This Project

### Step 1: Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### Step 2: Navigate to the project directory

```bash
cd zomato-restaurant-eda
```

### Step 3: Install the required libraries

```bash
pip install -r requirements.txt
```

### Step 4: Download the dataset

Download the original `zomato.csv` file from the Google Drive link and place it inside:

```text
data/raw/
```

### Step 5: Open the Jupyter Notebook

```bash
jupyter notebook
```

Open `notebooks/Zomato_EDA_Analysis.ipynb` and run the analysis cells.

## 📚 Key Learnings

Through this project, I gained practical experience in:

- Data exploration using Pandas.
- Identifying and handling missing values.
- Data quality assessment.
- Univariate, bivariate, and multivariate analysis.
- Data visualization using Matplotlib and Seaborn.
- Outlier detection using IQR and Z-Score methods.
- Correlation analysis.
- Feature engineering and data transformation.
- Translating analytical findings into business recommendations.

## 📝 Conclusion

This project demonstrates the use of Python for end-to-end Exploratory Data Analysis.

By analyzing restaurant ratings, pricing, cuisines, customer engagement, and service availability, the project identifies meaningful patterns and potential business opportunities.

The analysis highlights how data exploration and visualization can support better business understanding and data-driven decision-making.

---

**Project:** Zomato Restaurant EDA

**Category:** Data Analytics | Exploratory Data Analysis

**Technologies:** Python | Pandas | Matplotlib | Seaborn
