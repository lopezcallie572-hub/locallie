# README.md
#Market Insight Generator

## Overview

The Market Insight Generator is a Python analytics system that evaluates market categories using:
- Real-world product data
- News sentiment analysis
- Google Trends interest data

It outputs a ranked list of market opportunities along with a visual chart and PDF report.

---

##  APIs Used

### 1. Fake Store API
- URL: https://fakestoreapi.com/products
- Purpose: Provides product categories used as market segments

### 2. NewsAPI
- URL: https://newsapi.org/
- Purpose: Retrieves recent news headlines for each category
- Authentication: API key required

### 3. MeaningCloud Sentiment API
- URL: https://www.meaningcloud.com/
- Purpose: Performs sentiment analysis on news headlines
- Authentication: API key required

### 4. Google Trends (pytrends)
- Purpose: Measures public interest over time for each category
- No API key required

---

## Authentication

API keys are stored in `config.py`:

```python
NEWS_API_KEY = "your_key"
MEANINGCLOUD_KEY = "your_key"
