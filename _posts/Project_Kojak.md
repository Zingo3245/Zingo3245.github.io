---
layout: post
title: Project Kojak: Predicting the source of news articles
---

# Predicting the source of news articles

As we've seen since 2016, there have been news articles coming from many questionable sources. 

## Data

Building off the previous project, I scrapped from a wider variety of sources for a total of 11 which representing the political left, right, and center as well as conspiracy/fake websites. In order to scrape websites effectively I made scripts which were sent up to my EC2 instance on Amazon AWS. Each of the scripts was run on a different core in order to parallelize the process. All of the articles were fed into MongoDB.

## Model

With the articles on my local machine, I first tagged the parts of speech and dropped the nouns so I could train my model on the writing style. I also took the stem of the words so different variations of words were put together when the articles are broken up into a word matrix. After I created a corpus, I trained a random forest classifer on the data which was over 70% accurate. 

## Conclusion

I was able to build a model that was good at distinguishing the source of news articles. At the same time I was able to create a pipeline for handling large scale processes. 