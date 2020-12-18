+++
title = "Filtering Methods"
description = "The algorythms that employ their users."
date = 2020-11-25T02:13:50Z
author = "Beate Zirdziņa"
+++

## What is it? 
**Collaborative filtering** uses previously acquired historical data on user behaviour and
interactions between users and items to predict their preferences. This method is either aimed more at
items – for example on Amazon, all the products have many buyers who most probably also buy other
things. Products often bought together would thus be filtered in a group. The other option is user profile analysis – in this case the algorithm would look for users with similar “shopping carts” – these include
both current and past purchases, to determine which users share similar habits. CF can also be further
divided into memory–based or model–based filtering. “Memory–based approaches rely on pairwise
similarities between vectors of ratings, while model–based approaches rely on factorizing the entire
rating matrix.”[^1] Both of these models can be employed for an item based or user profile–based filtering. 

**Content-Based Filtering** methods, as the name suggests, focus on content key words and the descriptions
provided for items on web–pages to analyse which target audiences would enjoy them. This method
does not usually employ interaction between the content consumers. Recommendations using this
method are made by analysing the type of content being filtered and looking for items most similar to it.
As Zarzour et al. suggest, content–based filtering is widely used in a variety of domains ranging from
recommending webpages, news articles, restaurants, etc. For examples: Pandora Radio recommends
songs that share similar characteristics and Rotten Tomatoes recommends users with movies that share
similar cast and storyline. This filtering method falls short, however, if the descriptions and information provided for items
to be recommended is lacking.


[^1]:H. Zarzour; Y. Jararweh; Z. A. Al-Sharif; (2020) An Effective Model-Based Trust Collaborative Filtering for
Explainable Recommendations; from the 11th International Conference on Information and Communication Systems
(ICICS); Jordan.