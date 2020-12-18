+++
title = "Recommender Systems – What are they?"
description = "A short theoretical introduction to recommender systems."
date = 2020-11-20T02:13:50Z
author = "Beate Zirdziņa"
+++

## A Little Bit of Theory

Recommendation systems find their origins in various areas of artificial intelligence and
mathematics, such as approximation theory, cognitive systems, information retrieval, prediction
methods, and management science. Among a wide assortment of choices recommendation systems use
the “input” of users – which in this context means just the community using the particular service – to
determine interest groups and help incoming community members find content in line with their
preferences more easily. Since the mid 90’s recommendation systems have cemented their place as a
separate research area.[^1]

The need for recommendation systems becomes more and more apparent and essential taking
into account the massive avalanche of information accessible via the Internet, not to mention the fact
that the amount of information grows exponentially every moment. With this oversaturation of content
users may find it more and more difficulties to reach the internet artefacts and information they want.
Sometimes users don’t really even know what it is they are looking for – most often the case with
Netflix and other watchable content especially. Different websites employ various solutions to cope
with the problems of information filtering and data mining. Not to mention the fact that with new user's
their preferences must be determined first. Up and coming and new items must be rated by the
community as well. One user can only conceivably rate a small number of items at a time, so the rating
matrix is sparse – the systems in place must be able to deal with the fact that similarities among groups
and communities must be determined in a meagre matrix.[^2]

The authors of “An Effective Model–Based Trust Collaborative Filtering for Explainable
Recommendations” describe that: “Memory–based collaborative filtering is one of the recommendation
system methods used to predict a user’s rating or preference by exploring historic ratings, but without
incorporating any content information about users or items. It can be either item–based or user–based.”
There are two steps to be taken to employ item–based Collaborative Filtering (CF) predictions:
1. **Select pair–based similarities** – a variety of items similar to the content the user has
already rated to be good.
2. **Use users expressed opinions** – be it through views or ratings, comments and so on – on
these similar items to predict a rating for a predictor item.[^3]

Now, the websites that employ this system do not do it out of the goodness of their heart and just
to improve the user experience – which, admittedly is very important in its own right. The purpose of it
is largely to lead to greater sales, longer watch time, more service subscriptions and more time spent on
the website in question – which, most of the time, also means more time for ad–placement. For example,
Hafed Zarzour et al. point out that “data gathered for three weeks in the summer of 2001 showed that
between 20% and 40% of sales on Amazon are due to recommended products that do not belong to the
shop’s 100,000 most sold products, and 60% of movies rented by Netflix are selected based on
personalized recommendations.” Recommendation systems also have the added benefit of showing the
user categories on the periphery of their interest which may lead to them discovering even more content
they’re ready to pay for.
Recommendation systems usually produce a list of recommendations in one of three ways:
1. Collaborative Filtering,
2. Content–based Filtering,
3. Hybrid of These Two Approaches.[^4]

[^1]: O. B. Fikir; I. O. Yaz; T. Özyer; (2010). A Movie Rating Prediction Algorithm with Collaborative Filtering; from
International Conference on Advances in Social Networks Analysis and Mining; Denmark
[^2]: Same as previous.
[^3]: D. Wang, Y. Yih, M. Ventresca (2020) Improving neighbor-based collaborative filtering by using a hybrid similarity
measurement.
[^4]: H. Zarzour; Y. Jararweh; Z. A. Al-Sharif; (2020) An Effective Model-Based Trust Collaborative Filtering for
Explainable Recommendations; from the 11th International Conference on Information and Communication Systems
(ICICS); Jordan