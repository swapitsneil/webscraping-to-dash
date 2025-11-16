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

## Features

Web Scraping: Fetches 15 pages of ASUS laptops using requests and BeautifulSoup.
Data Cleaning: Parses prices (e.g., "₹49,990" → 49990) and reviews (e.g., "1,000 Ratings&75 Reviews" → separate numeric columns).
Feature Engineering: Creates business KPIs like:
Price Category (Budget, Mid-Range, etc.)
Popularity Score (weighted ratings + reviews)
Value Score (rating × log(ratings) / price)
Engagement Ratio (reviews / ratings)
Price per Rating and more.

EDA & Insights: Generates stats like average price (₹48.9K) and top models.
Power BI Dashboard: Visualizes:
Price range distribution (Pie Chart).
Ratings vs Reviews trend (Line Chart).
Top trusted laptops (Bar Chart).
Popularity by category (Bar Chart).


## Business Problems Solved

1) Which price range sells most? → Mid-Range dominates (25% share).
2) Are expensive laptops worth it? → Value Score reveals overpriced models.
3) Which models have highest trust? → Top 10 by ratings (e.g., Expertbook P1).
4) Price vs Quality sweet spot? → ₹42K at 4.4 rating.
5)Segment competitiveness? → Competitive_Intensity by price band.
6) Best marketing ROI? → High engagement + low price/rating.

## Technologies Used
Python 3.11: Core scripting.
Libraries: requests, BeautifulSoup (scraping), pandas (cleaning/EDA), numpy.
Tools: Jupyter Notebook for development, Power BI for dashboard.
Data: ~300 ASUS laptop records from Flipkart.

## Installation
1) Clone the repo:
         git clone https://github.com/swapitsneil/webscraping-to-dash.git
         cd webscraping-to-dash

2)   
