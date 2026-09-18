# Google Play Store — Exploratory Data Analysis

An end-to-end EDA on the Google Play Store dataset (~10,000 apps) and a companion User Reviews dataset (~64,000 reviews), uncovering what drives app ratings, installs, and pricing on the Play Store.

## 📌 Problem Statement

The Play Store is home to millions of apps competing for attention, but developers often lack clear, data-backed guidance on which categories to target, how app size and pricing affect installs, and how user sentiment reflects an app's reception. This project analyzes real Play Store data to answer those questions.

## 🎯 Business Objective

- Identify which app categories have the highest demand and which are under-served
- Understand how size, pricing, and content rating relate to ratings and installs
- Check whether review sentiment aligns with app ratings
- Provide actionable recommendations for launching or improving an app

## 🗂️ Dataset

- `Play Store Data.csv` — app-level metadata (category, rating, size, installs, price, etc.)
- `User Reviews.csv` — user reviews with sentiment labels

> Source: [Google Play Store Apps dataset (Kaggle)](https://www.kaggle.com/datasets/lava18/google-play-store-apps)

## 🧹 Data Cleaning

- Removed 483 duplicate rows and 1,181 duplicate app entries
- Fixed an invalid Rating value (> 5)
- Converted Reviews, Size, Installs, and Price from text to numeric types
- Standardized "Varies with device" sizes as null
- Converted Last Updated to datetime

## 📊 Key Findings

- **Categories:** Family, Game, and Tools are the most crowded by app count; Game, Communication, Tools, Productivity, and Social drive the most installs
- **Ratings:** Most apps cluster around a 4.3 rating; 92.2% of apps are free, 7.8% are paid
- **Size vs. Installs:** Larger app sizes correlate with fewer installs — smaller, optimized apps perform better
- **Reviews vs. Rating:** Review count is a much stronger predictor of installs than star rating alone
- **Sentiment:** The majority of user reviews are positive

See the full notebook for all 13 charts, insights, and business-impact discussion.

## 🛠️ Tools & Libraries

Python · Pandas · NumPy · Matplotlib · Seaborn

## 🚀 How to Run

1. Clone this repo
   ```bash
   git clone https://github.com/YOUR-USERNAME/play-store-eda-project.git
   ```
2. Install dependencies
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. Open `Play_Store_Project.ipynb` in Jupyter Notebook / JupyterLab and run all cells

## 💡 Recommendations

1. Target under-served, high-engagement categories (e.g. Events, Beauty, Parenting) or high-rated niches (Education, Weather, Art & Design)
2. Keep app size lean to reduce install friction
3. Prioritize driving review volume, not just chasing a higher star rating
4. Price paid apps under $10 unless there's a strong premium differentiator
5. Track review sentiment over time as an early warning signal for quality issues

## 👤 Author

**Shamim Ahmed**
[LinkedIn](https://www.linkedin.com/in/shamimahmed444/) · ahmedshamim0126@gmail.com
