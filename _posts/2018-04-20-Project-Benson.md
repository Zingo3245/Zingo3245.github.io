---
layout: post
title: Project Benson: Using MTA subway data to predict interest for a gala
---

#Metis Project Benson
For our first project, Victoria Ng and I were enlisted to help the fictional group WomenTechWomenYes(WTWS) with a gala they are planning to hold. To recruit people, WTWS would send street teams to subways in New York City and wanted our help with figuring out which stations would be the most optimal placement for their teams.

##Data
The main requirement for the project was that we use the New York Metropolitan Transportation Authority(MTA) data but were also highly encouraged to bring in other data. The MTA data was a challenge to clean as there were various formatting issues. Our first step was to check our dates to see if there were any outliers and we noticed that 3/11 and 3/17-3/23 registered relatively low counts so we decided to remove these from the data. We also decided to remove irregular counts as well as non-regular audits. Once we dealt with these issues, we were ready to bring in some outside data.

We also decided to check the American Community Survey(ACS) conducted by the Census. The ACS data was able to provide us with data for how many people held PhDs within a certain zip code. We decided that areas with a higher number of PhD holders would yield a higher number of interested participants for the WTWY gala. We first isolated the zip codes column and the column that contained the amount of PhD holders per zip code. We then filtered the data with the zip codes for New York City.

##Model

Using the top 90th percentile of busiest stations in the MTA Data and the top 15 zip codes of PhD holders yielded 35 stations for each list. From there we were able to pick out 11 stations that were in both lists. Our recommendations were that WTWY focus their efforts on those 11 stations.