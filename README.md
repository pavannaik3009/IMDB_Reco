During the last few decades, with the rise of Youtube, Amazon, Netflix and many other such web services, recommender systems have taken more and more place in our lives. From e-commerce (suggest to buyers articles that could interest them) to online advertisement (suggest to users the right contents, matching their preferences), recommender systems are today unavoidable in our daily online journeys.

A **recommender system** is a subclass of information filtering system that seeks to predict the "rating" or "preference" a user would give to an item. They are primarily used in commercial applications.

#### There are 2 types of recommender systems:

**Collaborative recommender systems** aggregate ratings or recommendations of objects, recognize commonalities between the users on the basis of their ratings, and generate new recommendations based on inter-user comparisons.

**Content-based recommender systems** learns a profile of the new user’s interests based on the features present, in objects the user has rated. It’s basically a keyword specific recommender system here keywords are used to describe the items. 

<p align="center" ><img width="500" alt="Screen Shot 2019-11-24 at 1 40 23 AM" src="https://user-images.githubusercontent.com/43712046/69491476-766eb100-0e5b-11ea-8fa7-6bfc781045a8.png"></p>


In this project we have combined movie attributes such as genre, plot, director and cast to calculate its cosine similarity with another movie to build a movie recommender system.


## Web Scraping
Tools: Python(Beautifulsoup, re)

Web scraping, web harvesting, or web data extraction is data scraping used for extracting data from websites.

**re(regular expression)** is a special sequence of characters that helps you match or find other strings or 
sets of strings, using a specialized syntax held in a pattern.

**Beautifulsoup** is a library for pulling data out of HTML and XML files.

There are four main object types in Beautifulsoup: Beautifulsoup Object, tag object, NavigatableString object and Comment object.

We need to call the HTML doc initially and set it equal to IMDB markup.
Here is an example of scraping the Movie Name from the IMDB website. 

<img width="1440" alt="Screen Shot 2019-11-21 at 3 13 12 PM" src="https://user-images.githubusercontent.com/43712046/69583705-1da93080-0fa1-11ea-98db-726c2c12d243.png">

The entire code for scraping the Top-250 movies from IMDB can be found [here.](https://github.com/pavannaik3009/IMDB_Reco/blob/master/WebScraping.ipynb)

We have scraped the **Movie Name, Director, Release Date, Running time, Country, Language, IMDB Rating, Genre, Number of votes, Plot, Cast** from IMDB website. 


## Data Cleansing
Tools: Python(pandas, numpy, re)

The scraped data has many features that needs to be cleaned. It can be seen that there are missing values in Language with a 'See more' value and the language of that movie is actually present in the Country column. Therefore, we need to coreect these my index mapping. 

Also, Release Date has the values of the Country taht needs to be dropped and only the year needs to be extracted from dd/mm/yyyy format.

The year is in string format that needs to be converted to integer values. 

The running time values needs to be converted to minutes from hh:mm. 

The IMDB rating is a float value and not a string value. It needs to be converted.

The notebook for Data Wrangling can be found [here.](https://github.com/pavannaik3009/IMDB_Reco/blob/master/DataWrangling.ipynb)

## Data Visualization

## Feature Selection

## Recommender system
