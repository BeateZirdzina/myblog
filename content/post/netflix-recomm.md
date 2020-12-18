+++
title = "The Netflix Recommender System"
description = "How do They Know?!"
date = 2020-12-04T02:13:50Z
author = "Beate Zirdziņa"
+++
## What's the Deal, Netflix?
It is well known that most consumers do not *really know* what they want. Countless research papers have illustrated that the more choices the person is faced with, the harder and more exhausting the choosing process becomes and the more likely it is that the user will - in the end - come to the “none of the above” choice - choose not to choose! Neil Hunt et. al. (2015) explains that “Consumer research suggests that a typical Netflix member loses interest after perhaps 60 to 90 seconds of choosing, having reviewed 10 to 20 titles on one or two screens. The user either finds something of interest or the risk of the user abandoning the service increases substantially”. So, the recommendation system is crucial at this moment – to make a quality suggestion high enough on the user’s page as to not lose them entirely.

{{<figure src="../img/img6.png">}}

How the Netflix homepage and all subsequent page’s work is they display a “titular” content piece at the top – this may be a new release or something that the user would most likely like to watch. Under this titular item the content is divided into rows of mutually similar items, such as action movies, new releases, comedies and so on. Typically, each home page has about 40 rows. Let’s take a look at the typical rows Netflix offers:[^1]

1. **Personalised Video Ranker (PVR)** – Videos in these rows usually are produced by the same algorithm. These are typically genre rows such as “Horror”, “Action” and so on. Content in these rows, as the name suggests, is ordered by the users’ unique preferences, so 2 users with the same interest row may get completely different results. This row is also supplemented with site–wide popular content and new releases to drive users to rate items outside their centre preferences.
2. **Top–N Video Ranker** – For example “Top 10 in Latvia”. This row is mostly the same to all users as it calculates the Top content in a general sense. 
3. **Trending** – There are two types of trends that this algorithm can identify: 
* Set time repeating trends – For example if Christmas is coming, the trending row will display Christmas movies, while around February we would probably observe romantic comedies and the like.
* Short term trends – Display users short term interest. For example, at the start of the virus pandemic, this algorithm would find movies that cover the topics of quarantine and pandemic because those are the top topics all around the web.
4. **Continue Watching** – Since Netflix offers many episodic shows the user can easily check this row to get back to right the moment, they saw last. This also works if a movie watching session is interrupted.
5. **Because You Watched (BYW)** – This is a non–personalised algorithm that simply gathers similarly ranked movies. Despite the fact that the algorithm itself is not personalised, the movie chosen for BYW is personalised, so a user that prefers horror would receive similar horror movies to watch. 

{{<figure src="../img/img4.png">}}

The homepage generator uses all of these algorithm–based rows altogether to produce the most likely sequence of rows so that the user would find something they like as close from the top of the page as possible. Netflix also take into account the fact that users’ moods and needs change as well as the likely chance that one account is used by multiple people at once so the wide selection of different rows makes it more likely that each user will find something they like.

[^1]: C. A. Gomez-Uribe, N. Hunt (2015) The Netflix Recommender System: Algorithms, Business Value,
and Innovation. ACM Trans. Manage. Inf. Syst. 