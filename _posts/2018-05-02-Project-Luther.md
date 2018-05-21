---
layout: post
title: Project Luther: Using video game data to predict user's ratings of video games
---

# Metis Project Luther

I was interested in predicting how users would rate a video game based on the user score. Video games have become a big busniess that are projected to be worth an estimated $215 billion in 2018. To get the data to examine the issue, I turned to the popular video game selling website Steam.

## Data

In order to get the data from Steam and it's accompanying website Steam Spy, I would have to take the data from the web pages with Selenium. Scrapping Steam was difficult due to the complexity of different game pages where some games had age blockers or other games were part of a collection. This made it impossible to use a single method to find the data on every game. As the project went on, I later discovered a Kaggle dataset that also contained features that I could use to predict video game ratings so I downloaded that as well. 

## Model

The first model was the data comprised from the data gathered from Steam and Steam spy. In this model, I predicted that price and number of owners a game had would accurately predict the each user's rating of the game. I used Lasso Regression which helped me pair down redundant features from my model. Unfortunately the model had no predictive power and suffered from high error rates.

I decided to test a second model that was gathered from the Kaggle Data had a different set of features but could still be trained on user rating. In this model, I predicted that Critic's ratings, the number of critics who reviewed a game, the year the game was released, and the global sales of a game would predict the game's user rating. This model actually did have predictive power and had reasonably low error rates. 

## Conclusion

The model that relied on data from Steam and Steam spy may benefit from more data points. That model only had 100 rows of data and if there were an easier way to scrape the websites, more data could be gathered and the predictive power of the model increased. One of the advantages of the second model was that it had several thousand cases. The second model could benefit from more features in order to increase it's predictive power. 