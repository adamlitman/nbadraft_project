# NBA Draft Pick Classification (python): Project Overview
- Created a classifier for determining whether an NBA player was drafted too high, too low, or accurately
- Scraped data for over 2900 draft picks from basketballreference.com from 1981 through 2010
- Added ranking features to determine the optimal draft order for each year based on player success
- Explored and visualized the data using multiple plot types in seaborn and matplotlib
- Built and tested multiple classification techniques to find the optimal model (K-nearest neighbors, Naive Bayes, Logistic Regression, Decision Tree)

## Sources and Code Used
- Data Source: https://www.basketball-reference.com/
- Article for building scraper: https://medium.com/hardwood-convergence/intro-to-virtual-environments-and-scraping-nba-data-with-beautifulsoup-6ce745f8c26e
- Python Packages Used: pandas, BeautifulSoup, requests, matplotlib, numpy, seaborn, sklearn

## Web Scraping
Modified the scraper in the article above to pull 30 years of NBA Draft data. For each draft selection, I scraped the following columns:
- Pick Number
- Player
- Team
- College
- Years Played
- Games Played
- Minutes Played
- 14 additional player statistics such as points per game, total rebounds, WinShares, Box Plus/Minus, etc.

## Data Cleaning and Modifications
- Made column for draft year
- Converted relevant columns to numeric type
- Filled all null values
- Created a key to standardize team acronyms for teams that changed locations 
- Standardized the data by including only top 60 picks for each draft year
- Added columns to rank players in each draft by WinShares, VORP, and BPM
- Added columns to identify lottery picks and superstar players
- Added columns to identify if players were picked too high or low based on ranking features

## Exploratory Data Analysis

