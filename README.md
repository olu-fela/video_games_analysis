# video_games_analysis

# TripleTen Data Science Sprint 5 Integrated Project - Vide Games Sales Analysis

## Introduction
This project analyzes video game sales and associated data to identify patterns that determine a game's success. The dataset contains information on user and critic reviews, game genres, platforms (e.g., Xbox, PlayStation), and sales figures across various regions (North America, Europe, Japan, and other countries). It also includes content ratings assigned by the Entertainment Software Rating Board (ESRB).

The goal is to uncover actionable insights that can inform marketing strategies and identify potentially profitable platforms, genres, and regions. By analyzing historical data up to 2016, we aim to make data-driven recommendations for planning a successful advertising campaign in 2017.

This project takes a comprehensive approach, combining data cleaning, visualization, statistical analysis, and hypothesis testing to deliver insights that can inform game release strategies and marketing decisions.

## Dataset

The dataset includes:

<table>
  <thead>
    <tr>
      <th>Column Name</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**Name**</td>
      <td>Game title</td>
    </tr>
    <tr>
      <td>**Platform**</td>
      <td>Platform or console (e.g., Xbox, PlayStation, PC).</td>
    </tr>
    <tr>
      <td>**Year_of_Release**</td>
      <td>Year the game was released.</td>
    </tr>
    <tr>
      <td>**Genre**</td>
      <td>Game category (e.g., Shooter, RPG, Action).</td>
    </tr>
    <tr>
      <td>**NA_sales**</td>
      <td>Sales in North America (in millions of USD).</td>
    </tr>
    <tr>
      <td>**EU_sales**</td>
      <td>Sales in Europe (in millions of USD).</td>
    </tr>
    <tr>
      <td>**JP_sales**</td>
      <td>Sales in Japan (in millions of USD).</td>
    </tr>
    <tr>
      <td>**Other_sales**</td>
      <td>Sales in other regions (in millions of USD).</td>
    </tr>
    <tr>
      <td>**Critic_score**</td>
      <td>Average critic score (out of 100).</td>
    </tr>
    <tr>
      <td>**User_Score**</td>
      <td>Average user score (out of 10).</td>
    </tr>
    <tr>
      <td>**Rating**</td>
      <td>ESRB content rating (e.g., E, T, M).</td>
    </tr>
  </tbody>
</table>

Since the dataset for 2016 may be incomplete, earlier data trends are used to build a foundation for forecasting and planning for 2017.

## Steps and Approach

1. **Data Exploration**
    - Loaded the dataset and examined its structure, column names, and data types.
    - Investigated missing values, irregularities, and general patterns within the dataset.

2. **Data Preparation**
    - Standardized column naming conventions for consistency.
    - Converted columns to appropriate formats to facilitate accurate computations.
    - Addressed missing values using thoughtful imputation strategies:
        - Replaced placeholders like "TBD" with NaN.
        - Applied statistical measures such as medians to fill in gaps for numerical data.
    - Calculated total global sales as a sum of regional sales, introducing a new column total_sales.

3. **Data Analysis**
    - Studied trends in game releases by year to determine the relevance of the dataset for different timeframes.
    - Analyzed platform-specific performance to identify platforms with the highest sales and their growth or decline over time.
    - Created visualizations such as box plots to compare global sales distributions across platforms.
    - Examined correlations between review scores (critic and user) and sales for selected platforms, using scatter plots and statistical measures.
    - Explored the profitability of various game genres, identifying the most lucrative ones.

4. **Regional Sales Profiles**
    - Profiled user preferences in North America (NA), Europe (EU), and Japan (JP):
        - Determined the top five platforms for each region and analyzed market share variations.
        - Identified the top five genres and compared regional preferences.
        - Investigated the effect of ESRB ratings on sales in different regions.

5. **Hypothesis Testing**
    - Formulated and tested hypotheses to explore trends in user preferences:
        - Assessed whether average user ratings for Xbox One and PC platforms are statistically equivalent.
        - Evaluated whether average user ratings differ significantly between Action and Sports genres.
    - Applied t-tests with a significance level of 0.05 to assess hypotheses and provide evidence-based conclusions.

6. **Final Conclusions**
    - Summarized key findings across platforms, genres, and regional trends.
    - Highlighted actionable insights for boosting sales through effective platform selection, genre targeting, and regional campaigns.
    - Provided data-backed recommendations for optimizing advertising strategies in 2017.

