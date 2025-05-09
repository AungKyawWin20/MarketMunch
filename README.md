# MarketMunch: Data-Driven Restaurant Opportunity Analysis

## Overview

MarketMunch is a data-driven project that analyzes U.S. restaurant market conditions to help entrepreneurs and investors identify the best opportunities for opening new restaurants or takeout businesses. Using a combination of population, income, restaurant, and consumer trend data, the project answers key questions about where and what type of restaurant is most likely to succeed.

## Key Questions

- Which U.S. state has the best market conditions for a new restaurant or takeout business?
- What type of restaurant (e.g., fast food, casual dining, fine dining, ethnic cuisine) has the highest success rate?
- What demographic, economic, and consumer behavior factors influence restaurant success?

## Data Sources

- **Population Data:** U.S. Census Bureau (2020-2024)
- **Income Data:** U.S. Bureau of Economic Analysis (BEA)
- **Restaurant Data:** Yelp (via SerpApi)
- **Consumer Trends:** Google Trends (via SerpApi)
- **Cuisine Supply Data:** Yelp (via SerpApi)

## Project Structure


```
MarketMunch/
│
├── Datasets/
│   ├── Population Data (2020-2024).csv
│   ├── SAINC70_CA_2000_2023.csv
│   ├── SAINC70_TX_2000_2023.csv
│   ├── SAINC70_FL_2000_2023.csv
│   ├── california_restaurants_data.csv
│   ├── google_trends_data.csv
│   └── San Diego Cuisines Data.csv
│
├── project.ipynb
└── README.md
```

## How It Works

1. **Population & Income Analysis:**  
   Identifies states with the largest populations and highest income levels.

2. **Restaurant Data Collection:**  
   Scrapes Yelp for restaurant ratings, reviews, and types in major California cities.

3. **Consumer Trend Analysis:**  
   Uses Google Trends to analyze demand for different cuisines in target regions.

4. **Supply Analysis:**  
   Scrapes Yelp for the number and quality of restaurants by cuisine in San Diego.

5. **Visualization:**  
   Uses Seaborn and Matplotlib for clear, insightful visualizations.

## Insights

- **Best State:** California, due to high population and income.
- **Best City:** San Diego, for its high average ratings and engagement.
- **Best Restaurant Type:** Ethnic food, especially Thai and Indian, for their balance of demand and quality.
- **Market Gaps:** Korean and Burmese cuisines show high quality but lower supply, indicating potential opportunities.

## Getting Started

1. Clone the repository.
2. Install dependencies:
   ```bash
   pip install pandas matplotlib seaborn tqdm serpapi
3. Add your SerpAPI key as an environment variable
    ```bash
    export serp_api = YOUR_SERPAPI_KEY
4. Open `project.ipynb` and run the cells.

## Future Improvements

- Integrate social media data for deeper demand analysis.
- Incorporate demographic breakdowns by ethnicity.
- Expand to other states and cuisines.

## License

Apache 2.0

---

_Created by Aung Kyaw Win. Designed with ❤️ for modern data-driven retail teams._