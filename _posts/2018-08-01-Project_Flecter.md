---
layout: post
title: Project Flecter: Predicting bias in news articles
---

# Predicting Bias in News Articles

Ranking bias is a tough thing to do. People often believe that they are objective and that what conforms to their own viewpoints is free of bias. Websities such as [Media Bias/Fact Check](https://mediabiasfactcheck.com/) rely on raters to inform their readers of where different websites stand in terms of the bias of view points. Is there a way to use data to predict bias?

![news_matrix](/images/news_matrix.jpeg "news_matrix")

## Data

I scrapped 550 articles from Huffington Post, Breitbart, and Rueters. The articles were downloaded into a database in MongoDB and I had to drop rundandant articles that were swept up in the scrapping process. These articles were taken from each site's politics section since politics tends to be an area where there is a strong focus and clear definition of bias.

## Model

After cleaning the text I used Count Vectorizer to fit a matrix which was reduced down to three topics thanks to KMeans. These three clusters tended to correlate with their respective sources.

![Topics_KMeans_clusters](/images/news_matrix.jpeg "news_matrix")

## Conclusion

While the clusters did correlate with the source, there was a big issue that lingered. There was no way to define political bias based on the given data. The use of one source for each bias meant that the clusters found something distinct with the source but that did not necessarily mean it was on a right/left/center political spectrum. It was what lead me to my next project where I could gather articles from a greater variety of sources.