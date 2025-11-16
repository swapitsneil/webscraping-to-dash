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

## ⭐ Key Features
🕸️ 1. Web Scraping

Scrapes 15 pages of ASUS laptops using:
- requests
- BeautifulSoup
- Saved HTML pages to avoid repeated requests

🧹 2. Data Cleaning
- Converts price strings → integers
- Splits “Ratings & Reviews” text

🧠 3. Feature Engineering
Creates powerful KPIs used in analytics:
- Price Category (Budget, Mid-Range, Premium)
- Popularity Score
- Value Score
- Engagement Ratio
- Price per Rating

📊 4. EDA & Insights

Examples:

- Average ASUS laptop price → ₹48,900
- Sweet-spot pricing → ₹42K at 4.4★
- Mid-range laptops dominate 25% of listings and most rated ones
- Expertbook P1 ranks as a top-trust model

📈 5. Power BI Dashboard

Includes:
- Price distribution (Pie)
- Ratings vs Reviews trend (Line)
- Popularity by category (Bar)
- Top trusted laptops (Bar)
- Value Score comparison

## 🧩 Tech Stack
Languages
Python 3.11

Libraries
requests
beautifulsoup4
pandas, numpy

Tools
Jupyter Notebook
Power BI Desktop

## ⚙️ Installation

Clone the repository:

    git clone https://github.com/yourusername/asus-laptops-scraper.git
    cd asus-laptops-scraper

Install dependencies:

    pip install requests pandas numpy csv
    from bs4 import BeautifulSoup

Install Power BI Desktop (free):
Microsoft: https://powerbi.microsoft.com/desktop

## 🚀 Usage Guide
1. Run the Web Scraper
   Open:
      webscraping.ipynb

This notebook:
- Scrapes Flipkart pages
- Saves raw HTML inside /pages/
- Converts scraped data → structured DataFrame
- Exports laptops_cleaned.csv

2. Perform EDA & Feature Engineering

Continue the notebook to:
- Create KPIs
- Analyze ratings, prices, reviews

Plot optional graphs

3. Build the Power BI Dashboard
- Open Power BI
- Import laptops_cleaned.csv
- Add visuals:
Pie → Price Category
Bar → Top Models by Rating
Line → Ratings vs Reviews
Card → Avg Price & Avg Rating

## ❓ Business Questions Answered

| Question                          | Insight                              |
| --------------------------------- | ------------------------------------ |
| Which price range is most common? | Mid-Range dominates (25%)            |
| Which models are most trusted?    | Expertbook P1, Vivobooks             |
| Does higher price = better value? | Not always (Value Score proves this) |
| What is the sweet-spot price?     | ~₹42,000 with 4.3–4.4★               |
| Where is competition high?        | Premium category                     |


## ❤️ Acknowledgments

Flipkart (data source — educational use only)

BeautifulSoup

Power BI

⭐ If you found this project useful, consider starring the repository! 🌟
