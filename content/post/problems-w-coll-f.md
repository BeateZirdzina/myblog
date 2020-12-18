+++
title = "Some Problems With Collaborative-Filtering"
description = "Nothing is ever perfect"
date = 2020-11-28T02:13:50Z
author = "Beate Zirdziņa"
+++

# Some Problems With Collaborative Filtering

### Sparsity
When wanting to realise a recommender system one has to face the fact that they work best when
used with datasets the size of, for example, those that Netflix, Amazon and Facebook can offer – namely
huge datasets. The largest part of users would only review few of the offered items, but this is then
remedied by the fact that there are at the least tens of thousands of items and millions of users. H. Zazour
et.al. (2020) notes that “One of the typical challenges that could be introduced by data sparsity is the
Cold Start Problem. Since collaborative filtering methods make recommendations based on users’ past
preferences, new users need to rate a sufficient number of items in order to let the recommendation
system learn their preferences and make reliable recommendations.”[^1]

Collaborative filtering methods are largely unable to supply accurate recommendations if the
users have rated only a couple of items – this is to say that in such a situation the system has not received
enough input to get to know the user well enough to group them together with their *preference peers*.

### Scalability
Scalability problems arise when the number of users and items grow exceedingly large – this will
be a problem for traditional collaborative filtering method. Since model–based approaches use the entire
dataset to train, new user ratings have to be analysed in real time to make an updated recommendation.[^2]

However, fortunately in application, relative to the absolute number of items available for
consumption, most users only review comparatively few items, and thus memory–based methods can
react in a timely manner to new ratings and offer predictions in real time even when faced with extremely
large datasets. Model–based approaches can avoid scalability issues by employing dimensionality reduction techniques, however they may suffer from computationally expensive matrix factorization and
may lose useful information in the process. Thus, we can observe that there are some trade–offs to
consider between scalability and performance in model–based approaches.[^3]

### Dimensionality
The aim of collaborative filtering is to find similarities or patterns between content or consumers
to then conclude which content pieces / users are alike each other. Since there are a great lot of consumers
and content, pairwise similarities are calculated in high–dimensions. This brings us to something called
the Hughes Phenomenon or otherwise known as the peaking paradox – with a fixed size of training
samples, the predictive power reduces as the dimensionality increases. To put it simply, Hughes
observed that “measurements have a finite accuracy. The outcome of any set of measurements may
thereby be represented as a vector (point) in a finite, discrete space. As different measurements may lead
to the same representation point, this point may also be understood as a cell in which all indistinguishable
outcomes are collected.” Two outcomes may result:[^4]

1. Concentration – Similarities between all consumers or content blend together and become the
same. In this case memory–based collaborative filtering is unable to find the most similar content
or consumers, thus will not be able to make a reliable prediction.
2. Hubness – Some content occurs more frequently in the nearest neighbour lists of other content.
This content is usually highly rated and popular and does not contribute any unique, personal
preference information for recommendations due to the fact that this popular item may be liked
by many users. These ‘main–stream’ products or content can behave like noise making memory–
based collaborative filtering unable to make accurate predictions.

In the 2010 article *Hubs in Space: Popular Nearest Neighbours in High–Dimensional Data* published in the Journal of Machine Learning Research, Nanopoulos et al. explain that “memory–based
Collaborative filtering methods that use cosine–like similarity measurements to calculate pairwise
similarities suffer hubness and concentration problems caused by high dimensionality of the data.
Model–based methods with dimension reduction methods such as SVD cannot solve those problems
either.”

In order to reduce hubness one would have to reach intrinsic dimensionality, where any further
reduction may lead to loss of information. Concentration and hubness – contrary to sparsity or skewness of the distribution of rating – are inherent properties of high dimensionality. The accuracy of forecasts
can be adversely impacted by both phenomena, as they impair the representativeness of nearest
neighbour lists. Although reducing hubness will improve the efficiency of prediction by using reciprocal
proximity as a similarity calculation, the precision cannot rival the state–of–the–art model–based
approaches.[^5]

[^1]: H. Zarzour; Y. Jararweh; Z. A. Al-Sharif; (2020) An Effective Model-Based Trust Collaborative Filtering for
Explainable Recommendations; from the 11th International Conference on Information and Communication Systems
(ICICS); Jordan
[^2]: Same as previous.
[^3]: Same as previous.
[^4]: G. Hughes (1968) On the Mean Accuracy of Statistical Pattern Recognizers. Volume: 14, Issue: 1. IEEE
Transactions on Information Theory
[^5]: M. Radovanovi, A. Nanopoulos, M. Ivanovič (2010) Hubs in Space: Popular Nearest Neighbours in HighDimensional Data. Journal of Machine Learning Research