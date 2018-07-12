---
layout: post
title: Project Benson: Using MTA subway data to predict interest for a gala
---

# Metis Project Benson
For our first project, Victoria Ng and I were enlisted to help the fictional group WomenTechWomenYes(WTWS) with a gala they are planning to hold. To recruit people, WTWS would send street teams to subways in New York City and wanted our help with figuring out which stations would be the most optimal placement for their teams. 

## Data
In order to decide where to send the street teams, we would have to use the data from the New York Metropolitan Transportation Authority(MTA) on station usage. It was also highly encouraged that we bring in outside data to help with our analysis. The MTA data was a challenge to clean as there were various formatting issues. Our first step was to check our dates to see if there were any outliers and we noticed that 3/11 and 3/17-3/23 registered relatively low counts so we decided to remove these from the data. We found some strange anamolies with the counts. Some stations appeared to be counting backwards while the counts in other stations appeared to be thrown off by audits that were occuring outside of the regular four hour time intervals. We created a function to reverse the negative counts while dropping the audits from the data. Once we dealt with these issues, we were ready to bring in some outside data.

We decided that people with PhDs were be more willing and have more money to donate to the gala. To figure out how we could reach people with PhDs we decided to check the American Community Survey(ACS) conducted by the Census. The ACS data was able to provide us with data for how many people held PhDs within a certain zip code. We first isolated the zip codes column and the column that contained the amount of PhD holders per zip code. We then filtered the data with the zip codes for New York City.

## Model

Using the top 90th percentile of busiest stations in the MTA Data and the top 15 zip codes of PhD holders yielded 35 stations for each list. From there we were able to pick out 11 stations that were in both lists. Our recommendations were that WTWY send thier street teams to these 11 stations.

![Graph](https://github.com/Zingo3245/Zingo3245.github.io/tree/master/images/blue_bars.png "barh graph")