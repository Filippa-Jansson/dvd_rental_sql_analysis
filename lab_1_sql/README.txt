### Hello and welcome to my lab 1 in SQL!

#### I will write the comments of my coding here instead in the code just to make it look cleaner.

#### Imports-Here I use import on duckdb, pandas and matplotlib so I can use them in .ipynb file. I needed to have duckdb because it allows me to use SQL in Python. Pandas helps me to convert all the SQL data into Dataframes for analysis. Matplotlib helps with create the statisics bars for the codes, which is much nicer to see visually.


#### Movies longer than 3 hours- I use Select to find the columns that I want to display. FROM specifies with table i choose, which I chose film in  this case. The I use WHERE length > 180 to filter all the movies that are longer than 180 minutes.

#### Movies that involves the word love- I kind use the same coding as I did with the last one but I used WHERE lower(title) LIKE '%love%' to help me find all the movies that has the word love in

#### Statistic of movies length-Rinse and repeat like the others but I had to do some different coding to get the statistics from the data. I used MIN() to find the shortest movie they had, which is 46 min. AVG() helps to calculate the average length of all the movies in the data. MEDIAN() helps to find the middle value of all the movies and MAX() shows which movie is the longest one.

#### Top 10 expensive movie per day- Here I use rental_rate / rental_duration AS cost_per_day to sort and find the highest daily rental cost, also creating a temporary column name while doing it.

#### Actors that has played in most movies- I use JOIN to connect the actors to films category, then later on use I use GROUP BY to group up the results by actor. I laso use COUNT() to count how many films the actor has appeared in. Lastly I use ORDER BY just to organise the actors by the number of movies that exsits in the data. I also use LIMIT 10 so it shows the top 10 actors instead of all

#### Personal questions- So i chose using "Which category has the most movies and "Most rented out movie", I thought they were interesting and maybe good to show for "The manager".

#### First question- I use COUNT() to find out how many movies exists FROM category group. Then i JOIN the two groups to create a temporary column. I later use GROUP BY and ORDER BY to organise the categories and the amount of movies per category.

#### Second question- Kind of the same how I've been doing in all the other cells. I SELECT movies and use COUNT rentals to count how many movies has been rented out. I use GROUP BY and ORDER BY to organise it a bit and LIMIT it by 10.

#### Top 5 customers and Income per movie category- I will make a JOIN on these because I feel I'm repeating too much on the coding and these are the only one I've used matplotlib. Since I've imported myplotlib I use df...plot to create a statistic bar that shows the data better.

#### Comments- It was a very fun assignment and a bit tricky sometimes. I hope the assignment passes and I wish you a merry christmas!