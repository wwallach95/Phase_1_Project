# Microsoft Studios Research Project
**Author**: Wolfgang Wallach

## Outline
* [Overview](#Overview)
* [Business Project](#Business-Project)
* [Data](#Data)
* [Methods](#Methods)
* [Results](#Results)
* [Conclusions](#Conclusions)
* [More Information](#More-Information)
* [Repository Structure](#Repository-Structure)

## Overview
At the request of Microsoft Studios, I have conducted research into the modern day movie industry. Using Data from [IMDB](https://www.imdb.com/), [Box Office Mojo](https://www.boxofficemojo.com/), and [TheMovieDB.org](https://www.themoviedb.org/), I have compiled a few insights that should help the burgeoning studio get started along its path to success and relevance.

## Business Project
I had been tapped by Microsoft Studios, the Microsoft Corporations new movie studio, to help them decide which types of movies they should create. Using the data from IMDB, Box Office Mojo, and TheMovieDB.org, I plan to answer the following questions:
* [How can we define a successful movie?](./Question 1.ipynb)
    * Is it defined by how much money it makes?
    * Is it defined by the profitability of the movie?
    * Should a successful movie be judged by its rating?
* [Which genres are the most successful?](./Question 2.ipynb)
    * How much does it cost to make a movie in the most successful genre
    * Which genre has the greatest margin for profit?
* [Which movies are the easiest to make?](./Question 3.ipynb)
    * How many people does it take?
    * How much does it cost to make?
    * Are the easiest movies to make the most successful?
* Using the insights gained from the previous questions, what are the first few movies that the production company should make?

## Data
The data used for this project were a total of seven separate .csv files from the three aforementioned websites, IMDB, Box Office Mojo, and TheMovieDB.org. These are all websites that track movie data, and will be invaluable for this project. I will be focusing mostly on the movie staff, the review scores, and the production and gross values for each movie.

## Methods
Since I ended up working with seven different DataFrames, I had to do a fair amount of manipulation with pandas to get them to cooperate and join the way I wanted. Some data frames had titles, some had variables that represented the titles, and some had both. Thankfully there was at least one DataFrame that had the overlap, otherwise I would have had to join through other values, which would have been far more time consuming. Once I had the data formatted the way I wanted it, I was able to merge and join the DataFrames that were relevant for each question. Occasionally, I'd start answering a question and realize that I didn't had a DataFrame I needed, so I would need to do a bit more cleaning and merging to properly answer the question.

Ultimately, this approach worked out pretty well for me. Having cleaned and merged most of my data beforehand, I was able to tackle the questions without worrying too much about how I needed to wrangle my data so as to properly answer the questions.

## Results
Throughout the course of this project, I found the following answers to my questions:
* There are multiple ways to define a successful movie. As a base line, any movie that is profitable can be said to be successful, but for our purposes, we are going to say that any movie that grossed over 600 million dollars and also has an average review score of 6 or above is a successful movie. This will give us a threshold for what we want our movies to accomplish.
* The most successful genres, animation, musical, and science fiction, are not the most prolific. This should help Microsoft Studios make movies that aren't going to have as much competition as some of the more prolific genres, but also allow for a greater profit margin.
* Unfortunately, determining the ease of making a movie was a little difficult, and also revealed that the movies that are the easiest to make generally don't do as well as the movies that are more difficult, ie. Movies that cost more to make and require more people to make.

## Conclusions
Having gone through the data and crunched some numbers, I can safely recommend that the first movies that Microsoft Studios should make should be a science fiction movie, and an animated musical. The goal will be to have both of these movies meet the criteria defined earlier for a Successful Movie. In order to ensure that resources are not spread too thin and the movies can receive the full attention of the studio, Microsoft Studios should limit itself to just these two movies.

Going forward, I would like to look into release date patterns to determine when best to release the two movies, as well as looking into foreign markets, as this project focused solely on the domestic market.

## More Information
Please review my full analysis in our [Jupyter Notebook](./) or our presentation.

For any additional questions, please contact me at **wwallach95@gmail.com**

## Repository Structure

* Data-----------------------------------------------------(Folder of cleaned data in .csv format)
* Graphs--------------------------------------------------(Folder of graph images)
* PDFs----------------------------------------------------(PDFs of the workbooks)
* zippedData--------------------------------------------(Folder of the zipped, non cleaned data)
* Data Import and Cleaning.ipynb-----------------(Main data cleaning workbook)
* Question 1.ipynb-------------------------------------(Question 1 workbook)
* Question 2.ipynb-------------------------------------(Question 2 workbook)
* Question 3.ipynb-------------------------------------(Question 3 workbook)
* Consulting proposal.pdf----------------------------(Powerpoint Presentation PDF)
