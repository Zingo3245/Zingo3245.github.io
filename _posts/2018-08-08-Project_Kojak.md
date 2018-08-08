---
layout: post
title: Project Kojak: Predicting the source of news articles
---

# Predicting the source of news articles

As we've seen since 2016, there have been news articles coming from many questionable sources. An important component to trying to fight fake news is to track how information is spreading. The question is how can a data science apporach be used to figure out the source of news articles.

## Data

Building off the previous project, I scrapped from a wider variety of sources for a total of 11 which representing the political left, right, and center as well as conspiracy/fake websites. In order to scrape websites effectively I made scripts which were sent up to my EC2 instance on Amazon AWS. Each of the scripts was run on a different core in order to parallelize the process. All of the articles were fed into MongoDB.

![Parallel_processing](/images/Parallel_processing.png "Parallel_processing")

## Model

With the articles on my local machine, I first tagged the parts of speech and dropped the nouns so I could train my model on the writing style. I also took the stem of the words so different variations of words were put together when the articles are broken up into a word matrix. After I created a corpus, I trained a random forest classifer on the data which was over 70% accurate. 

![Predicted_news_articles](/images/Predicted_news_articles.png "Predicted_news_articles")

## Conclusion

From my confusion matrix above, I noticed there were some interesting correlations. In my model, Brietbart was often confused with Infowars. This would make sense sense both are commonly thought to have a conspiracy theory style of writing.

![Breit-Info](/images/Breit-Info.png "Breitbart-Infowars_predictions")

It was also no surprise that Huffington Post was confused with Mother Jones as both are considered far left news sources.

![HuffJones](/images/HuffJones.png "HuffingtonPost-MotherJones_predictions")

What was surprising was that Huffington Post and Mother Jones were confused with Infowars. This could be because all of these sources have populist sources. Some have noted that at times the extreme left and extreme right have some convergence.

![Left_right_convergence](/images/Left_right_convergence.png "Left_right_convergence")

I was able to build a model that was good at distinguishing the source of news articles. At the same time I was able to create a pipeline for handling large scale processes. 