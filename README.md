# ASUS Laptops Web Scraper & Analytics Dashboard

## Project Overview
This project is a complete data pipeline for scraping ASUS laptop listings from Flipkart, cleaning the raw data, performing feature engineering, and visualizing key insights in a Power BI dashboard. It demonstrates web scraping, data processing, and business analytics using Python.

Date: November 16, 2025
Goal: Analyze ASUS laptop prices, ratings, and popularity to uncover business insights like "sweet spot" pricing and value for money.
Data Source: Flipkart product pages (scraped ethically for educational purposes).

Key outputs:

Cleaned CSV (laptops_cleaned.csv) with 300+ rows and engineered features.
Interactive Power BI dashboard for sales intelligence.

<img width="2012" height="1114" alt="Image" src="https://github.com/user-attachments/assets/fb86679c-3aa0-42fc-9575-c506fd69c0de" />

⭐ Key Features
🕸️ 1. Web Scraping

Scrapes 15 pages of ASUS laptops using:

requests

BeautifulSoup

Saved HTML pages to avoid repeated requests

🧹 2. Data Cleaning

Converts price strings → integers

Splits “Ratings & Reviews” text

Fills missing values

Removes duplicates

🧠 3. Feature Engineering

Creates powerful KPIs used in analytics:

Price Category (Budget, Mid-Range, Premium)

Popularity Score

Value Score

Engagement Ratio

Price per Rating

Competitive_Intensity

📊 4. EDA & Insights

Examples:

Average ASUS laptop price → ₹48,900

Sweet-spot pricing → ₹42K at 4.4★

Mid-range laptops dominate 25% of listings

Expertbook P1 ranks as a top-trust model

📈 5. Power BI Dashboard

Includes:

Price distribution (Pie)

Ratings vs Reviews trend (Line)

Popularity by category (Bar)

Top trusted laptops (Bar)

Value Score comparison
