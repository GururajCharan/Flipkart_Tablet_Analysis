# Flipkart Tablet Web Scraping &  Market Analysis 

An end-to-end data project that scrapes tablet information from Flipkart, followed by data cleaning and exploratory data analysis (EDA) to uncover key insights into the Indian tablet market.

## Project Goal
The primary objective of this project is to analyze the tablet listings on Flipkart to understand the market landscape. The analysis focuses on identifying patterns in pricing, brand popularity, feature distribution (like RAM and storage), and customer ratings.

## Methodology
The project follows a structured data analysis workflow:

1.  **Data Scraping**: A Python script using `Requests` and `BeautifulSoup` scrapes data from the first 20 pages of Flipkart's tablet search results. The script is designed to be robust against basic anti-scraping measures.

2.  **Data Cleaning & Preprocessing**: The raw scraped data is loaded into a `Pandas` DataFrame and undergoes a cleaning process, which includes:
    *   Handling missing or null values.
    *   Standardizing data types (e.g., converting price strings to numerical values).
    *   Extracting and separating features from text descriptions (e.g., parsing RAM, ROM, and display size).

3.  **Exploratory Data Analysis (EDA)**: The cleaned dataset is analyzed to answer key questions about the tablet market. This involves generating descriptive statistics and creating visualizations to highlight trends and relationships.

## Key Insights & Visualizations
*(This is the most important section. Replace the examples below with your actual findings and charts from your notebook.)*

*   **Brand Dominance**: Which brands have the most listings? Is there a difference between budget and premium segments?
    > *Example: Samsung and Apple dominate the premium price range (> ₹30,000), while Lenovo and Redmi have a strong presence in the budget-friendly category.*

*   **Price vs. Ratings**: Is there a strong correlation between a tablet's price and its customer rating?
    > *Example: Most tablets, regardless of price, have ratings between 4.2 and 4.6, suggesting that price is not the sole indicator of customer satisfaction.*

*   **Feature Analysis**: What are the most common RAM and storage configurations?
    > *Example: The most common configuration offered is 8GB RAM with 128GB ROM, indicating a market shift towards higher-spec mid-range devices.*

## Tools and Libraries
*   **Language**: Python
*   **Data Manipulation**: Pandas
*   **Web Scraping**: Requests, BeautifulSoup
*   **Development**: Jupyter Notebook

## How to Reproduce
To run this project on your local machine, follow these steps:

1.  **Clone the repository:**
    ```
    git clone https://github.com/your-username/flipkart-tablet-analysis.git
    cd flipkart-tablet-analysis
    ```
2.  **Install the required libraries**:
    ```
    pip install pandas requests beautifulsoup4 jupyter
    ```
3.  **Run the Jupyter Notebook**:
    Open and run the `Tablet_Analysis_WebScrapping.ipynb` notebook to see the full analysis.

## Future Improvements
*   **Sentiment Analysis**: Perform sentiment analysis on customer reviews to gain deeper insights into product strengths and weaknesses.
*   **Price Tracking**: Scrape data periodically to track price fluctuations and identify sales trends.
*   **Comparative Analysis**: Expand the scraping to other e-commerce sites (like Amazon) to perform a comparative market analysis.

