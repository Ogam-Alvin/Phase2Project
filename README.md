# MOVIE STUDIO ANALYSIS

![christian-chen-P1cMlvl_yGk-unsplash](https://github.com/user-attachments/assets/8b7ba4d9-de1e-4ddd-a04c-361e5f66edee)


## Project Overview
This project will use exploratory data analysis to generate insights for a business stakeholder.

## Business Problem

Since the client sees big companies creating original video content and they want to get in on the fun, they want to create a new movie studio. 
The aim of this project is to make tangible business suggestions on movie producton on what types of films are currently doing the best at the box office. This process will involve analysing different movie datasets to gain more information and enable better bussiness suggestions to the client. These findings must then translate  into actionable insights that the head of the company's new movie studio can use to help decide what type of films to create.

The main business questions this project sought to answer were:
 * What is the total profit made by movies based on the genres and which genres have the most profit

 * What are the most popular genres among customers?
 * Which season(s) is best to release a movie in order to maximize profits.

 ## Data Understanding and Analysis
 For this project we will be having 6 data sources:

1. bom.movie_gross.csv: This is a file that contains information regarding a movies name, both domestic and foreign gross amount and the year it was released

2. im.db:This is a zipped folder that contains a database called im which contains data regarding a movie. This data includes what category it falls under, the direcctor, actors involved, movie ratings, running time and many more

3. rt.movie_info.tsv: This file has information the movie rating for theatrical releases e.g. 'R' 'PG 13' e.t.c. it also tells more about the movie like genre, director, theatrical release date, dvd release date, runtime, box office gross and studio
4. rt.reviews.tsv: This is a list of reviews from reviewers and and the ratings they gave, it also gives info on who published the review

5. tmdb.movies.csv: Here we have genre ids, movie titles, language the movie is in, its popularity, release date,vote count and the average vote

6. tn.movie_budgets.csv: This file contains a movies production budget, domestic gross and worlwide gross

# Data Description
In order to take a closer look at the data sources, all the necessary libraries were first imported. All the above datasets were then loaded  and analyzed to gain better insight on the data. One of the files was a zipped file which had to be unzipped first in order to access the data within it.
After loading the datasets, it was easier to find related columns that could be used to connect two or more tables.

The total gross profit by genre was determined using a series of code and the results displayed in a graph as shown below for better visualization:

![Screenshot 2024-07-28 152833](https://github.com/user-attachments/assets/b860cbb0-3770-4b52-8c2b-81b3ae7e98be)

The most popular movie genre among customers was analyzed by looking at the ratings given for different movies. The best way to obtain this information was merging the movie_basics table with the movie_ratings table. To display the results, this bar graph showing popularity of Genres by Count was plotted. 

![Screenshot 2024-07-28 153633](https://github.com/user-attachments/assets/57d1d0bf-2b0a-4582-822c-44baebbfe380)

From the graph above it was noted that:
* There is no other genre more popular than drama due to its large following
* The top 5 genres with a reasonable popularity count are : Drama, Documentary, Comedy, Thriller and horror, while only the first three have a popularity count of over 15k

The most appropriate time to release a movie in order to make the most amount of profit was analyzed by looking at the movie budgets table. A line graph showing the average profits of each month over the years was plotted as shown for better visualization.
![Screenshot 2024-07-28 154124](https://github.com/user-attachments/assets/88bb3a3d-d9a3-41ea-a2c0-8f43004e1cbb)

From the above graph we can deduce that;
* There is high growth in interest in between the month of April and May and the same for October to November
* Movies released in the months May,June,July and November have yielded the most gross profits.
* Movies released in January,April,Aug,September and October have yielded the least profits.


## Conclusion
The questions we sought to answer from the analysis were all answered and these are the relevant conclusions drawn. 
1. For the question on the total profit made by movies based on genres, we found that these are the most profitable genres to start with:
* drama
* adventure
* action
* comedy
* fantasy

The company will be able to match or excede the production budget of movies that fall in these genres.

 2. For the question on the most popular movie genre among customers, we considered the vote count of the genres and their average ratings across all movies found in a specific genre. From the vote count of the genres it was a clear indication that the drama genre had the most amount of fans, followed by documentary and comedy genres. As for the average rating it was easy to spot that the genres were all roughly having the same range in the ratings and the difference was not so significant

3. When detremining the most appropriate time to release a movie in order to make the most amount of profits, it was clear that there were two peak seasons when the amount of profit increased dramatically . The first was from the begining of April towards May, after which we then saw that over June and Jully the amount of profit was fairly high . The second peak period was from October to November but unfortunately it was evidence of the decline in profit from November to December. So from that analysis the best time to release a movie would be in the months of April and November,

Recomendations
* It is advisable to start with a middle tier movie genre such as Thriller, Sci-Fi or Animation, as a way to build raport among customers and to build the name of the company's studio, since the company will be venturing into the movie business as a beginner. 

* Release dates for any movies to be made in the months of April and October since those have beeen seen to have a rise in profits.
