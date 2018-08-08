---
layout: post
title: Project McNulty: Predicting the outcome of disputes between countries
---

# How to predict the outcome of disputes between countries

I've always been interested in international politics but one of the hardest arguements in this subject is debating how international conflicts will be resolved. It's an important issue since conflicts can rapidly spiral out of control and have tremedous costs.

## Data

I downloaded the dataset from the [Militarized Interstate Disputes(MID)](http://cow.dss.ucdavis.edu/data-sets/MIDs) website. The MID dataset is part of the Correlates of War Project that provides information about conflicts. The data set provides incidents between states from 1816 to 2010. The data was easy to clean and load into PSQL. I decided to join two different parts of the MID data: the first one which looked at each incident and the second part which looked at each state involved in the dispute. 

## Model

I had a problem building a model around predicting an outcome since I had an unbalanced dataset with the outcome 'Stalemate' making up 65% of all outcomes. I decided to compensate for this by splitting the analysis into two levels. I created a column with a binary classifier where 1 was a stalemate outcome and 0 represented all other outcomes. In the second level of analysis I built a model to predict all the other outcomes. 

![Confusion_stalemate](/images/Confusion_stalemate.png "Confusion_matrix_stalemate")

The first model was accurate in predicting stalemate was accurate 89% of time time while the model that predicted all other outcomes was accurate 77% of the time.

![Confusion_outcome](/images/Confusion_outcome.png "Confusion_matrix_outcome")

## Conclusions

Overall both models were very accurate but more data pertaining to non-stalemate outcomes would be desireable. There have also been criticisms of the MID dataset where some researchers recommend dropping some of the cases. 