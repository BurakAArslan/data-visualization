# Steam Data Visualization Dashboard

Interactive Streamlit app for exploring a game store dataset using rich Plotly visualizations and practical filters. The dashboard surfaces insights across downloads, ratings, pricing, tags, and platform/language support.

## Dataset

- File: `data/bestSelling_games.csv`
- Columns used: `game_name`, `developer`, `release_date`, `release_year`, `estimated_downloads`, `all_reviews_number`, `reviews_like_rate`, `rating`, `price`, `difficulty`, `length`, `age_restriction`, `user_defined_tags`, `supported_os`, `supported_languages`, `other_features`, `is_free`.
- Ensure the dataset meets course requirements (≥ 2,000 rows, ≥ 7 columns).

## Quick Start

1. Install Python 3.10+.
2. Install dependencies:
   ```bash
   pip install streamlit plotly pandas numpy
   ```
3. Run the app:
   ```bash
   streamlit run trae_app.py
   ```

## Visualizations

- Bar chart
- Treemap
- Parallel coordinates
- Scatter/Bubble
- Sunburst
- Sankey Diagram
- Violin
- 3D scatter
- Icicle

###### Bar Graph

* Technique: Bar chart
* Insight: Shows the top games by estimated downloads. Useful to quickly see which games are the most popular.

###### Treemap

* Technique: Treemap
* Insight: Shows downloads hierarchy by developer → free/paid → game. Reveals which developers dominate, and how free vs paid games contribute to downloads.

###### Parallel Coordinates

* Technique: Parallel coordinates
* Insight: Compares numeric features (downloads, rating, price, length, difficulty) across multiple games. Highlights patterns and correlations among top games.

###### Scatter/Bubble

* Technique: Scatter plot with bubble size
* Insight: Plots price vs rating, bubble size = downloads. Helps identify how price relates to rating and which games are highly downloaded.

###### Sunburst

* Technique: Sunburst chart
* Insight: Shows genre → developer → game with weighted downloads. Reveals which genres are most popular and which developers dominate top genres.

###### Violin

* Technique: Violin
* Insight: Whether “All Ages” games tend to accumulate more downloads than “Teen 13+” or “Mature 17+”.

###### Sankey Diagram

* Technique: Sankey
* Insight: Shows flow from Age Restriction → Genre → Price Type, highlighting which age groups prefer which genres and whether those genres are mostly free or paid.

###### Icicle Chart

* Technique: Icicle chart (hierarchical bar)
* Insight: Shows hierarchy of age restriction → primary genre → game. Helps understand which age groups dominate which genres and top games within those.

###### 3D Scatter

* Technique: 3D scatter plot
* Insight: Plots difficulty, length, rating in 3D for top games. Helps see clusters of similar game profiles and differences in design complexity.
