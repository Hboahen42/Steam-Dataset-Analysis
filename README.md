# Steam Top Games Analysis - CS433 Final Project

This project explores a dataset of the top 1,495 games on Steam (as of April 2026) to understand market trends, player preferences, and pricing strategies. It includes a full data analysis pipeline from raw data loading to predictive modeling using linear regression.

## Project Overview

The analysis is structured into five main sections, each focusing on a different stage of the data science workflow:

1.  **Data Loading and Overview**: Initial inspection of the dataset, identifying data types, and checking for missing values.
2.  **Exploratory Data Analysis (EDA)**: Visualizing distributions of prices, review scores, and genres. Exploring correlations between numeric features.
3.  **Data Cleaning and Wrangling**: Handling missing values, parsing complex fields (like ownership ranges and release dates), and engineering new features.
4.  **Aggregation and Insights**: Answering key business questions such as the most recommended games and average prices/reviews by genre.
5.  **Linear Regression Modeling**: Building and evaluating a model to predict game prices based on features like release year, genre, and popularity metrics.

## Key Findings

*   **Pricing Trends**: Game prices cluster at psychological anchors ($4.99, $9.99, $19.99, etc.). Racing and Massively Multiplayer games tend to have the highest average prices, while Casual and Indie games are more affordable.
*   **Quality vs. Popularity**: Counter-Strike 2 dominates recommendations with over 5 million, significantly higher than any other title. Most top-performing games maintain a positive review ratio above 75%.
*   **Predictive Modeling**: A linear regression model was built to predict game prices. The strongest predictor was found to be the **release year**, reflecting inflation and rising development costs.
*   **Model Limitations**: The model achieved an R² of 0.19, indicating that Steam pricing is heavily influenced by business decisions (budget, marketing, publisher strategy) not captured in the dataset.

## Dataset Details

The dataset (`steam_top_games_2026.csv`) contains 1,488 rows and 29 columns after initial processing, covering:
*   Pricing and discounts
*   User reviews and recommendations
*   Playtime metrics
*   Platform support (Windows, Mac, Linux)
*   Developer, publisher, and genre information
*   Estimated ownership ranges

## Technologies Used

*   **Python**: Primary programming language.
*   **Pandas & NumPy**: Data manipulation and numerical processing.
*   **Matplotlib & Seaborn**: Data visualization and plotting.
*   **Scikit-learn**: Machine learning (Linear Regression, Scaling, Cross-validation).
*   **Jupyter Notebook**: Interactive environment for the analysis.

## Getting Started

### Prerequisites

Ensure you have Python installed. You can install the required dependencies using pip:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### Running the Analysis

1.  Clone this repository to your local machine.
2.  Navigate to the project directory.
3.  Open the `steam_project_final.ipynb` notebook in Jupyter or your preferred IDE.
4.  Execute the cells sequentially to reproduce the analysis and results.

## Project Structure

*   `steam_project_final.ipynb`: The main notebook containing the full analysis.
*   `data/`: Directory containing the raw and cleaned datasets.
*   `models/`: (Optional) Directory for saved model objects.
*   `README.md`: Project documentation.
