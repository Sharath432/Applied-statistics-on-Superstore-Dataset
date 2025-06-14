Superstore Marketing Data Analysis
Overview
This repository contains a comprehensive analysis of the Superstore Marketing Data dataset, focusing on customer demographics, spending habits, and campaign responses. The project includes data cleaning, descriptive statistics, probability distributions, customer segmentation, and actionable marketing recommendations, implemented in Python using Google Colab. Visualizations and insights help identify customer segments and optimize marketing strategies.
Project Objectives

Clean and preprocess the dataset to ensure data quality.
Analyze customer demographics and spending patterns using descriptive statistics.
Model variable distributions (e.g., Normal, Binomial) to predict behaviors.
Segment customers into distinct groups based on characteristics and spending.
Deliver visualizations and recommendations to enhance marketing campaigns.

Dataset

File: Superstore Marketing Data.xlsx (original), cleaned_superstore_data.csv (processed).
Columns: Includes Age, Income, Education, Marital_Status, Total_Spent, NumWebPurchases, Response, Recency, and more.
Source: Hypothetical superstore customer data for marketing analysis.
Note: The original dataset is not included due to size; cleaned_superstore_data.csv is provided.

Tasks and Deliverables

Task 1: Data Cleaning and Feature Engineering
Cleaned missing values, outliers, and inconsistencies.
Engineered features: Total_Spent, Income_Category.
Output: cleaned_superstore_data.csv, demographic visualizations (e.g., age_histogram.png).


Task 2: Descriptive Statistics
Calculated mean, median, mode, variance, and standard deviation for key variables.
Identified outliers using IQR method.
Outputs: task2_descriptive_stats.csv, box plots (e.g., boxplot_income.png).


Task 3: Probability Distributions
Modeled Age (Normal), Income (Log-Normal), NumWebPurchases (Poisson), Response (Binomial).
Calculated probabilities and expected values.
Outputs: task3_distribution_summary.csv, distribution plots (e.g., age_distribution.png).


Task 4: Insights and Customer Segmentation
Explored relationships (e.g., Income vs. Total_Spent correlation).
Segmented customers into 4 clusters using K-means.
Outputs: grouped_spending_stats.csv, segment_summary.csv, visualizations (e.g., segment_scatter.png).


Task 5: Conclusion and Recommendations
Created visualizations for segment profiles, response rates, and demographics.
Provided recommendations (e.g., target high-spending segments with premium offers).
Outputs: recommendations.txt, summary_report.txt, visualizations (e.g., segment_spending_bar.png).



Repository Structure
superstore-marketing-analysis/
├── data/
│   └── cleaned_superstore_data.csv
├── scripts/
│   ├── task1_data_cleaning.py
│   ├── task2_descriptive_statistics.py
│   ├── task3_probability_distributions.py
│   ├── task4_insights_segmentation.py
│   └── task5_conclusion_recommendations.py
├── outputs/
│   ├── task1/
│   │   ├── age_histogram.png
│   │   ├── education_bar.png
│   │   └── marital_status_bar.png
│   ├── task2/
│   │   ├── task2_descriptive_stats.csv
│   │   ├── boxplot_age.png
│   │   └── boxplot_income.png
│   ├── task3/
│   │   ├── task3_distribution_summary.csv
│   │   ├── age_distribution.png
│   │   └── numwebpurchases_distribution.png
│   ├── task4/
│   │   ├── grouped_spending_stats.csv
│   │   ├── segment_summary.csv
│   │   ├── correlation_heatmap.png
│   │   ├── elbow_plot.png
│   │   └── segment_scatter.png
│   └── task5/
│       ├── segment_spending_bar.png
│       ├── response_by_segment_bar.png
│       ├── education_distribution_bar.png
│       ├── income_vs_spent_segment_scatter.png
│       ├── recommendations.txt
│       └── summary_report.txt
├── README.md

Requirements

Python Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, scipy.
Environment: Google Colab or local Python environment (Python 3.7+).
Install dependencies:pip install pandas numpy matplotlib seaborn scikit-learn scipy



How to Run

Clone the Repository:git clone https://github.com/your-username/superstore-marketing-analysis.git
cd superstore-marketing-analysis


Upload Data:
Place cleaned_superstore_data.csv in the data/ folder.
If starting from Superstore Marketing Data.xlsx, run task1_data_cleaning.py to generate cleaned_superstore_data.csv.


Run Scripts:
Open Google Colab or a local Jupyter notebook.
Execute scripts in order (task1_data_cleaning.py to task5_conclusion_recommendations.py).
Example in Colab:!pip install pandas numpy matplotlib seaborn scikit-learn scipy
%run scripts/task1_data_cleaning.py


Outputs (CSVs, PNGs, text files) are saved in outputs/ subfolders.


View Results:
Check visualizations in outputs/ (e.g., segment_spending_bar.png).
Read recommendations.txt and summary_report.txt for insights.



Key Insights

Demographics: Customers are ~48 years old, mostly with Graduation (50%) or PhD (20%) education, and Married (60%).
Spending: High-income customers (Segment 0) spend ~$1200, with a strong Income-Total_Spent correlation (0.62).
Behavior: Campaign response rate is 15%, highest in Segment 0 (20%).
Segments: Four clusters identified, from high-income, high-spending to young, low-spending customers.

Recommendations

Target high-spending segments (0, 1) with premium offers.
Engage low-spending segments (2, 3) with discounts to boost online purchases.
Personalize campaigns to improve response rates in segments 1–3.
Leverage education (Graduation, PhD) for tailored marketing.
Optimize e-commerce for Segment 0’s high web purchases.

Contributing
Feel free to fork this repository, submit issues, or create pull requests to enhance the analysis. Suggestions for additional visualizations or models are welcome!
Acknowledgments

Built using Python, Google Colab, and open-source libraries.
Inspired by marketing analytics best practices.

Contact
For questions or feedback, reach out via GitHub issues or email: [rsarath16new@gmail.com].
