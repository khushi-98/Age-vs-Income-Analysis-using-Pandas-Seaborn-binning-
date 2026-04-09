📊 Age vs Income Analysis using Pandas & Seaborn

This project demonstrates how to analyze the relationship between Age and Income using Python libraries like Pandas, Matplotlib, and Seaborn. It includes data grouping, visualization, and statistical insights.

🚀 Project Overview

In this project, we:

Create a dataset of Age and Income
Group data into meaningful categories
Visualize distributions using plots
Analyze income trends across age groups
🛠️ Technologies Used
Python 🐍
Pandas 📊
Matplotlib 📈
Seaborn 🎨
📂 Dataset

The dataset is manually created and contains:

Age: Ranges from 22 to 68
Income: Ranges from 30,000 to 100,000
⚙️ Key Steps
1️⃣ Data Creation

We create a DataFrame using Pandas:

df = pd.DataFrame(data)
2️⃣ Age Grouping

We categorize ages into bins:

20–29
30–39
40–49
50–59
60–69
df['Age_Group'] = pd.cut(df['Age'], bins=age_bins, labels=age_labels)
3️⃣ Income Grouping

Income is categorized into:

Low
Medium-Low
Medium
Medium-High
High
df['Income_Group'] = pd.cut(df['Income'], bins=income_bins, labels=income_labels)
📊 Visualizations
🔹 Age Group Distribution
Count plot showing how data is distributed across age groups.
🔹 Income Distribution by Age Group
Boxplot showing income spread within each age group.
📈 Analysis

We calculate the average income per age group:

avg_income = df.groupby('Age_Group')['Income'].mean().round(2)
💡 Insight:
Income generally increases with age in this dataset.
Older age groups tend to have higher average income.
▶️ How to Run
Install required libraries:
pip install pandas matplotlib seaborn
Run the Python script:
python your_script_name.py
📌 Output
DataFrame with Age & Income groups
Countplot of Age Groups
Boxplot of Income vs Age Group
Average income statistics
🎯 Conclusion

This project is a simple yet powerful example of:

Data preprocessing
Feature engineering (binning)
Data visualization
Basic statistical analysis

Perfect for beginners in Data Science & Python 🚀

📢 Connect with Me
YouTube: @learn.pywithradhe
Instagram: @learn.pywithradhe
Telegram: https://t.me/learnpywithradhe
