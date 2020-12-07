# WSUV_DATA115 Personal Data Project
Fall 2020


## Motivation
Growing up I loved sports. I played basketball from third grade, all the way through high school. One of the things that coaches always attempted to engrain in our minds was that if you don’t make your free throws you’re not going to win games. This is voiced everywhere in basketball, all the way up to the NBA. It is especially emphasized in the playoffs -- when the games mean the most. So what do the numbers say? Were my coaches and seemingly everyone in the basketball world onto something or were they just relaying shoddy information throughout the years? Do free throws really help teams win late into the season? To answer this, I set out to see if I could find some statistics to correlate a higher free throw percentage with better playoff performance. 
## Data Sources
Common box score statistics are taken at every NBA game and recorded all throughout the season. These totals are made readily available at a number of websites like the NBA’s own website and ESPN’s website. I found the best website for downloading and manipulating data to be basketball-reference.com. They have NBA statistics going all the way back to the beginning of the league. For this project I used playoff data from 2015-2020 seasons and one dataset from the 2019-2020 regular season.  More specifically, I used free throw shooting percentage data from those seasons.
##Processing
These datasets were fairly simple to process. Basketball-reference.com has options on each of the datasets to convert them to complete .CSV files for easy analysis. So I simply copied these datasets and saved them as .CSV files and uploaded them to two different Jupyter Notebooks. All of the datasets had complete data with no inaccuracies so there wasn’t much data to be cleaned in that aspect. However, I had to download all of the statistics (FG%, rebounds, assists, turnover, etc.) for each playoff season I gathered data on. When I tried to make a scatter plot using both of these datasets, there was an issue with the graphs lining up. This was fixed by taking the raw data from each raw .CSV dataset and combining only the free throw percentages for the teams in Excel and deleting the other irrelevant columns. The dataset was then used to create the graph I needed in python/Jupyter Notebooks. 

The second notebook was created to further analyze the data. I took the raw data .CSV from each of the 2015-2019 playoffs and created a dataframe for each of them in the notebook to manipulate. None of the data needed to be cleaned here, but again I deleted the unused columns. This was done in Python in the Jupyter Notebook instead of Excel like the last notebook. 
## Visualization
I started my analysis by comparing the 2019-2020 playoff teams to their regular season performance to see how improvements to free throw percentages correlated to their playoff finish. The result shows that some of the top finishing teams had improvements, but they had low free throw percentages in both regular season and playoffs. This somewhat debunks whether good free throw shooting in the playoffs is very important. 

![2020 Top Playoff FT% performers vs. Their Regular Season FT% Performance](https://raw.githubusercontent.com/maxburchett/WSUV_DATA115/master/2020_Playoffs_vs_Regular.png)

## Analysis
With the visualization showing low to no correlation between better performance and FT%, I wanted to know if this trend continued throughout other recent seasons or if this past season was just a fluke. So I created a second visualization that overlaid the playoff free throw performance from the previous 5 seasons of the playoff teams. This visualization also points to free throw percentage not having strong correlation to playoff performance.
![](https://raw.githubusercontent.com/maxburchett/WSUV_DATA115/master/15_19_Playoff_FT.png)

## Conclusion
Once all is said and done, there is another key thing to consider. While basketball is a team sport, it is still filled with individual players. If you’re in the NBA you’re already the best in the basketball profession. But there are some players who are even more special, they just seem to have that “X-factor”. No matter what the stats say on paper, players like LeBron James can completely impact and sway a game’s outcome. There aren’t really any stats to accommodate for a force of this nature. I think that’s what makes sports like basketball so entertaining, because even with all of the stats and analysis, you still have to play the game to find a winner.
