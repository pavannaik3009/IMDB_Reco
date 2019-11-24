During the last few decades, with the rise of Youtube, Amazon, Netflix and many other such web services, recommender systems have taken more and more place in our lives. From e-commerce (suggest to buyers articles that could interest them) to online advertisement (suggest to users the right contents, matching their preferences), recommender systems are today unavoidable in our daily online journeys.

A **recommender system** is a subclass of information filtering system that seeks to predict the "rating" or "preference" a user would give to an item. They are primarily used in commercial applications.

#### There are 2 types of recommender systems:

**Collaborative recommender systems** aggregate ratings or recommendations of objects, recognize commonalities between the users on the basis of their ratings, and generate new recommendations based on inter-user comparisons.

**Content-based recommender systems** learns a profile of the new user’s interests based on the features present, in objects the user has rated. It’s basically a keyword specific recommender system here keywords are used to describe the items. 

<img width="697" alt="Screen Shot 2019-11-24 at 1 40 23 AM" src="https://user-images.githubusercontent.com/43712046/69491476-766eb100-0e5b-11ea-8fa7-6bfc781045a8.png">


In this project we have combined movie attributes such as genre, plot, director and cast to calculate its cosine similarity with another movie.
