Investigating TMDb dataset:

ABOUT PROJECT:

  -  In this project, I am investigating a TMDB movies dataset. 
  -  The dataset contains information of 10865 movies.
  -  The source of this data is www.kaggle.com. 
  -  The dataset contains information like details of budget, runtime of movies, revenue, vote_Avg, popularity, release_year etc of the movies.
  -  The dataset contains information on movies from year 1960 to 2015.
  -  Imported all the required libraries such as:-
     Pandas, NumPy, Matplotlib, Seaborn.



DATA FOR INVERSTIGATION:

The tmdb-movies.csv file contains the data to be worked on. 
The investigation of this data has been done in tmdb_khush.ipynb jupyter file.



ABOUT WRANGLING:

Rows have been deleted from budget_adj or revenue_adj have a value of '0' .
Duplicate rows are deleted from the dataset.
'0' is replaced with 'NaN' for average runtime.
Unnecessory columns have been removed such as imdb_id, budget, revenue, homepage, keywords, overview, production_companies, tagline.



POSED QUESTIONS ARE:
Q1. Overall analysis of different columns.
Q2. Computing Similiar Analytics: What are the movies with max and min
        - Popularity
        - Budget
        - Revenue
        - Profit
Q3. What are the top 10 movies by rating?
Q4. What is the Count of movies based on rating category?
Q5. What attributes do the most profitable movie have?
         -   Average duration of movies.
         -   Average Budget.
         -   Average revenue.
         -   Average profits.
         -   Which director directed most films?
         -   Whcih cast has appeared the most?
         -   Which genre were more successful?
         -   Which month released highest number of movies in all of the years? And which month made the most profit?
Q6. In which month we had the most movies making profits?
Q7. Genre wise, no. of movies released per year...
Q8. What is relationship between various parameters..



ANALYSIS:

* Out of given dataset only 3848 movies contained valid data.
* Jurassic World is the movie with max popularity of almost 33.
* Avatar movie has made most revenue.. Making a revenue of more than $2.8B
* Star Wars film has the highest profit in all, making over $2.7B
* Average runtime of all movies is approx 109 min.
* The top rated movies are The Shawshank Redemption and Stop Making Sense with a rating of 8.4.
* Movie_rating:
    Low 1100
    Below Average 938
    Above Average 907
    High 902
* No. of movies with profit greater than $50 million dollars : 1542
* Least no of profitable movies: January.. The month with max no of profitable movies December...
* The least profitable month: Jan..  June and December were the months with max profit...
* No of movies released genre wise:
     Drama 1752
     Comedy 1357
     Thriller 1202
     Action 1084
     Adventure 749
* Correlations:
    Popularity has STRONG correlation with vote_count and GOOD correlation with profit and revenue_adj.
    Profit has STRONG correlation with revenue_adj and vote_count and GOOD correlation with popularity and budget_adj.
    Runtime, budget_adj and vote_average does not has good correlation with any parameter.
    Revenue_adj has Very Strong correlation with profit

Q. If I wanted to show one of the best and most profitable movie, who would I hire as director and cast, which genre would I choose and also at what month would I release the movie in?
Ans. I would..
          Choose any director from this - Steven Spielberg, Clint Eastwood, Tim Burton, Robert Zemeckis, Tony Scott
          Choose any cast from this - Tom Cruise, Tom Hanks, Brad Pitt, Robert De Niro, Sylvester Stallone
          Choose these genre - Drama, Comedy, Action, Thriller, Adventure
          Choose these release months - May, June, July, November, December.
          Choose budget range between $224 to  $368371256




LIMITATIONS of the dataset and analysis:

1. There is no normalization or exchanges rate or currency conversion is considered during this analysis and our analysis is limited to the numerical values of revenue, budget etc.

2. We have not considered type of vote positive or negative or any other value.

3. Dropping missing or Null values from variables of our interest might skew our analysis and could show unintentional bias towards relationship being analyzed.

4. Due to wrangling lot of movie data needed to be removed, so our analysis is limited to partial no. of movies. ( Only those movies whose data was valid and without any null values...)

5. There were lot of movies where the budget_adj or revenue_adj have a value of '0' which means that the values of those variables had not been recorded. Calculating the profits of these movies would lead to inappropriate results. So we needed to delete those rows.

6. Also this dataset had one duplicate row. We had to remove that duplicate row for setting one column(here id) as the index of whole dataset.

7. Unnecessory columns needed to be removed such as imdb_id, budget, revenue, homepage, keywords, overview, production_companies, tagline. This was done because either these contained large no. of null values or didn't seem promising enough to be fit for some analysis.




WHAT DID I LEARN?

After completing the project, I :
* know all the steps involved in a typical data analysis process.
* am comfortable posing questions that can be answered with a given dataset and then answering those questions.
* know how to investigate problems in a dataset and wrangle the data into a format that can be used.
* have practiced communicating the results of the analysis.
* am able to use vectorized operations in NumPy and Pandas to speed up your data analysis code.
* am familiar with Pandas Series and DataFrame objects, which lets access data more conveniently.
* lastly but not least,I  know how to use Matplotlib and Seaborn to produce plots showing findings.



REFFERENCES:

- Stack overflow.com
- Python documentation
- Matplotlib.org
- Datacamp.org
- Pythonprogramming.net