# Cricket-Analytics-for-T20-World-Cup-2024

# 1. Data Extraction and Web Scraping
   
# Working:

The script fetches match data from ESPNcricinfo using the requests library.

It uses BeautifulSoup to parse HTML and extract relevant match details from tables.

Scorecard links for individual matches are identified and stored for further player-level analysis.

# Importance:
Automates the process of gathering large-scale cricket data, reducing manual effort.

Ensures real-time updates and accurate player statistics for informed decision-making.

# 2. Data Cleaning and Transformation
   
# Working:

Extracted match data is stored in a structured format using Pandas.

Unwanted characters, empty values, and inconsistencies are removed.

Data is saved as a CSV file to facilitate further analysis.

# Importance:
Clean and structured data ensures accurate analytics and reliable insights.

Helps in standardizing the dataset, making it compatible for visualization and modeling.

# 4. Player Performance Extraction

# Working:

The script extracts batting and bowling stats for each player from individual scorecards.

It stores runs, wickets, strike rates, economy rates, and other key metrics in a dictionary.

These statistics are compiled into a DataFrame for further computations.

# Importance:

Provides a detailed breakdown of individual player performances.

Helps in comparing players based on multiple criteria, including batting and bowling efficiency.

# 5. Calculating Key Cricket Metrics

# Working:

Batting-related metrics like Batting Average, Strike Rate, Boundary Percentage, and Balls Faced are computed.

Bowling-related metrics like Bowling Average, Strike Rate, Economy Rate, and Balls Bowled are derived.

# Importance:

Helps in determining the most impactful players based on statistical performance.

Ensures data-driven player selection rather than relying on subjective opinions.

# 6. Role-Based Player Classification

# Working:

Players are categorized into different roles based on performance:

Opener: High runs, high strike rate, and aggressive batting style.

Anchor: Stable batsman with a good average and long innings.

Finisher: High impact in fewer balls, useful in death overs.

All-rounder: Significant contributions in both batting and bowling.

Fast Bowler: High wicket-taker with low economy and strike rate.

Custom formulas assign scores to players based on role-specific conditions.

# Importance:

Ensures the best-suited players are selected for each role.

Helps in balancing the team structure for optimal performance.

# 7. Selecting the Best 11 Players

# Working:

The top-performing players for each role are selected using nlargest() function.

Ensures at least one wicketkeeper and a minimum of three full-time bowlers are included.

The best player based on Overall Score (batting + bowling impact) is designated as the Captain.

# Importance:

Helps in forming a well-balanced team with specialists in each role.

Ensures that player selection is based on actual performance, not just reputation.

# 8. Exporting and Visualizing Data

# Working:

The final selected team is saved as a CSV file.

Tableau is used to create dashboards showcasing key player statistics and performance trends.

# Importance:

Provides clear visual insights into player performances.

Helps analysts, coaches, and cricket enthusiasts in making data-driven decisions.
