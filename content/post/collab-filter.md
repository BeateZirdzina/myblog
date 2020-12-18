+++
title = "Collaborative Filtering"
description = "We are all more alike than we think..."
date = 2020-11-26T02:13:50Z
author = "Beate Zirdziņa"
+++

# Collaborative Filtering

A key advantage of collaborative filtering over content–based filtering is that this approach studies the interactions between individuals or items without incorporating in–depth information of items and users. Thus, this method does not require background knowledge about the actual context or extensive information about the object in order to make recommendations. This system can essentially make a prediction without “understanding” a movie, a person, or music, etc. Thus, this approach can be applied broadly regardless of the contents of the data. However, it does require users to consume and rate content to begin with which may be a problem if the website is experiencing a cold start which is to say they may be beginning from zero users, but collaborative filtering works best with many users, many items and many ratings.[^1]

Collaborative filtering can employ two types of filtering models – **memory–based** and **model–based**. Both of these approaches have their own advantages and setback.

{{<figure src="../img/asd.png">}} [^0]

**A Memory–based approach** is effective and relatively easy to implement where one calculates similarities between items or users and uses them as weights on ratings to represent how much the opinions on items a user has rated can represent a user’s opinion on the unrated item. 

“A typical example of this approach is K–Nearest–Neighbour (KNN). First, item–based memory–based CFs find similar items by calculating pairwise similarities between the predicting item and all other items the user has
rated. These pairwise similarities are used to rank how representative of the predicting item each other item is. Therefore, the prediction accuracy of collaborative filtering algorithms is highly dependent on how accurate the similarity measurement is. Second, K most similar items to this predicting item are selected from the items that this user has already rated on and then it combines the user’s opinions of those K items by weighted average or weighted sum to predict a rating for the unrated item from the user. Such approaches are widely used due to their simplicity, explainability and effectiveness, and predictions can be made in real time as new rating data is added. However, its prediction accuracy decreases when few items have been rated. Its scalability is also limited for large datasets.”[^2]

{{<figure src="../img/img1.png">}}

**Model–based approach** employs data mining and machine learning algorithms to develop and train predictive models. There are many different algorithms (ex. Singular–Value Decomposition (SVD), Principal component analysis (PCA)) which use matrix factorization techniques. The model– based approach usually uses Dimensionality reduction to improve the scalability and accuracy. This solves the sparsity and scalability problems and thus this method performs better in prediction accuracy in comparison to memory–based CFs. But the models usually takes more time to build and train compared to memory–based approaches. Moreover, there exists a risk of losing useful information due to dimensionality reduction.[^3]

**The Hybrid model** combines two or more techniques, or combines one of the previously mentioned with other techniques such as deep learning or clustering to overcome the individual limitations and improve the performance such as prediction accuracy, scalability. However, this combining increases the computational complexity such as time and resources required.[^4]

[^0]: Source - https://towardsdatascience.com/various-implementations-of-collaborative-filtering-100385c6dfe0
[^1]:F.O.Isinkaye; Y.O.Folajimi; B.A.Ojokoh; (2015) Recommendation systems: Principles, methods and evaluation;
Volume 16, Issue 3, Egypt.
[^2]:Same as 1.
[^3]:Same as 1.
[^4]:H. Zarzour; Y. Jararweh; Z. A. Al-Sharif; (2020) An Effective Model-Based Trust Collaborative Filtering for
Explainable Recommendations; from the 11th International Conference on Information and Communication Systems
(ICICS); Jordan
