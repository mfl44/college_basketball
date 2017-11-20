### Project : Web Scraping and Data Visualization with NCAA Data (Work in progress)

- Web scraper to collect team name, logo, historical performance data 
- Image processing to find the dominant color of each team's logo for color coding in data visualization
- Data visualization of historical coaches' poll performance 


### Data visualization examples

#### Tableau - College Basketball Dashboard

https://public.tableau.com/profile/mike.landron#!/vizhome/NCAA_Basketball/AdvancedTeamPerformanceMetrics16-17Season
Dashboard containing various advanced college basketball statistics and data visualizations:

1) Breakdown of Team Scoring by Type of Shot
- Stacked bar chart showing how many 2-point, 3-point, and free throws each team made

2) Assisted vs. Unassisted Field Goals Made (FGM)
- Stacked bar chart showing how many assisted field goals/shots a team made vs how many unassisted field goals/shots

3) Advanced Team Performance Metrics
- Assist Ratio: (SUM([Assists]))/((SUM([Field Goal Attempts])+(SUM([Free Throw Attempts])*.44))+SUM([Assists])+Sum([Turnovers]))
- Effective Field Goal %: (SUM([Field Goals])+(.5*SUM([3-Point Field Goals])))/SUM([Field Goal Attempts])
- Pure Point Rating: Team metric of same name based on John Hollinger's Pure Point Rating for individual players; shows a team's ability to handle the ball and make good decisions on offense
- Rebound Rate: (SUM([Total Rebounds]))/(SUM([Total Rebounds])+SUM([Opponent Total Rebounds]))
-Turnover Ratio: (SUM([Turnovers]))/((SUM([Field Goal Attempts])+(SUM([Free Throw Attempts])*.44))+SUM([Assists])+Sum([Turnovers]))

4) Wins by Conference
- Packed Bubble chart showing the total number of wins for each conference

#### Plot.ly - Historical Coaches' Poll Data Graph by Conference (ACC Shown) (Work in Progress)

 
<div>
    <a href="https://plot.ly/~ml44/178/" target="_blank" title="plot from API" style="display: block; text-align: center;"><img src="https://plot.ly/~ml44/178.png" alt="plot from API" style="max-width: 100%;width: 600px;"  width="600" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a></div>

The graph shows the cumulative points of coaches poll data starting from 2003. Graph's color coding was determined by teams' dominant logo colors from image processing. Please click image above to see the interactive chart. 

General Observations/Musings: 
- Duke and North Carolina (UNC), two teams often perceived to be in the same "league" in terms of prestige & performance over time, actually have a significant performance gap. While Duke's performance (using the coaches' poll as a proxy) has been consistently good to excellent over time, 3 periods of inconsistency in UNC's performance (early 2005- early 2007;early 2010- late 2011; late 2012- late 2013) have caused them to fall significantly behind Duke despite having won more national championships in the examined time frame (3 for UNC vs 2 for Duke)
- Virginia on the rise: Despite the program being mired in mediocrity for most of the examined time frame, Virginia's program has risen from "basement-dweller" status to 6th in the ACC. This was largely do to consistently excellent performance starting at the end of 2014 through the present. Performance tapered off at the end of 2017 and it will be interesting to see if they can regain their form and further ascend.
- Notre Dame's inability to string together multiple good seasons has left them behind, with the majority of their points coming from only 4 seasons out of the 15 considered. This inconsistency us what has been holding Notre Dame back and preventing the school from making the jump from a "Good" to a "Great" basketball school.


 
