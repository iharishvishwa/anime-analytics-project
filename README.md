# Anime Popularity Analytics

## Project summary
Goal: Identify factors (genre, episode count, popularity, type) that influence an anime's rating and popularity.

1. Dataset
- Source: Kaggle — Anime Recommendations Database
- Files used: `anime.csv`, `rating.csv`
Rows (anime): 12064
Columns (anime): 11
Rows (ratings): 7813737
Columns (ratings): 3

Rating distribution
   - Mean rating: 6.47
   - Median rating: 6.57
   - Distribution shape: left-skewed(skew = -0.54)
   - Interpretation: Ratings are slightly left-skewed, which means more anime score on the higher side (6–8 range), with few extremely low-rated shows.

2. Top 5 most popular anime (by members)
1. Death Note — members: 1,013,917 — rating: 8.71  
2. Shingeki no Kyojin — members: 896,229 — rating: 8.54  
3. Sword Art Online — members: 893,100 — rating: 7.83  
4. Fullmetal Alchemist: Brotherhood — members: 793,665 — rating: 9.26  
5. Angel Beats! — members: 717,796 — rating: 8.39  


3. Popularity vs Rating
Correlation between rating and members: 0.3879
Interpretation:
This indicates a moderately positive relationship — more popular anime tend to have higher ratings, but there are many exceptions.

Top popular anime with rating < 7
(Shows that are popular but not highly rated)
School Days — members: 279,183, rating: 6.17
Dragon Ball GT — members: 226,625, rating: 6.72
Chaos;HEAD — members: 174,337, rating: 6.62
Yosuga no Sora — members: 173,216, rating: 6.72
Dakara Boku wa, H ga Dekinai — members: 169,615, rating: 6.96

Highly rated but low-popularity (hidden gems)
Taka no Tsume 8: Yoshida-kun no X-Files — rating: 10.00, members: 13
Spoon-hime no Swing Kitchen — rating: 9.60, members: 47
Mogura no Motoro — rating: 9.50, members: 62
Kahei no Umi — rating: 9.33, members: 44
Yakusoku: Africa Mizu to Midori — rating: 9.25, members: 53


4. Episode group insights
Average rating by episode group:
Long Series (25–50): 6.96
Standard TV (13–24): 6.95
Very Long (50+): 6.85
Short Series (2–12): 6.54
Movie (1 episode): 6.21
 - Summary : Long-running series tend to have the highest average rating; movies tend to have the lowest average in this dataset.

5. Top genres
  a) Most common genres (top 10 by count)
      Comedy — 4575
      Action — 2768
      Adventure — 2316
      Fantasy — 2242
      Sci-Fi — 2036
      Drama — 1977
      Shounen — 1684
      Kids — 1598
      Romance — 1437
      Slice of Life — 1204
b) Highest-rated genres (top 10 by avg rating)
      Josei — 7.44
      Thriller — 7.38
      Mystery — 7.23
      Police — 7.12
      Shounen — 7.06
      Psychological — 7.01
      Military — 7.00
      Supernatural — 7.00
      Romance — 6.99
      Shoujo Ai — 6.97

6. Common genre combinations
    Action + Sci-Fi — 1,011 shows
    Adventure + Fantasy — 928 shows
    Comedy + Shounen — 925 shows
    Adventure + Comedy — 903 shows
    Action + Adventure — 871 shows
    Comedy + Fantasy — 851 shows
    Action + Comedy — 842 shows
    Action + Shounen — 772 shows
    Comedy + Romance — 753 shows
    Comedy + School — 737 shows



Key takeaways
  Longer series tend to be rated higher, while movies generally average lower ratings.  
  Popularity ≠ quality — correlation is moderate (0.3879), and there are many exceptions.  
  Thriller, Mystery, Psychological, and Josei genres rank among the highest in average rating.  
  Comedy, Action, and Adventure dominate as the most frequently made genres.  
  Many niche anime with **very few members** have exceptionally high ratings (hidden gems).  
  Clear opportunities for future enhancements:  
    - Use MAL API for fresh data  
    - Build a recommendation system  
    -  Add sentiment analysis from Twitter/Reddit



👤 Author
HARISH VISHWA  
Data Analytics Student  
GitHub: 

    
Files
- `notebooks/01_loading_data.ipynb` — data loading & cleaning  
- `notebooks/02_EDA.ipynb` — EDA and visualizations  
- `dashboard/` — (Power BI / Tableau / Plotly Dash files)  
