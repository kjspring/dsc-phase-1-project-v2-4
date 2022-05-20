# Microsoft Movie Studio Production Recommendations
       
## Overview
In 2021, digital, theatrical, and physical sales of movies were $136.5 billion globally and $36.8 billion in the United States. Digital sales account for 80% of revenue, theatrical sales are 12%, and physical media is the remaining 8%.

Microsoft is creating a new movie studio and wants to know what types of movies they should create to tap into this industry. This project will explore what types of movies are currently doing the best at the box office and recommend what types of movies Microsoft should create.

## Objective - Business Questions

* What movie genres should Microsoft Movie Studios focus on?
* When should these movies be released?
* How much should be budgeted for the production of each movie?

## Deliverables
* [Presentation:  Genre, Release Time, and Budget for Microsoft Movie Studio](https://docs.google.com/presentation/d/1FRCtFUkY__pndP7pPa4Z1vMWZ-83tGATsAjRPp5Ye9U/edit?usp=sharing)
* Jupyter Notebook
* GitHub Repository

## Repository Navigation
* [/img](./img) - contains image files
* [/img/fig](./img/fig) - stores plots and figures created with the analysis
* [/zippedData](./zippedData) - stores data used for this analysis
* [/license](./license) - contains the license information
* [project_notebook.ipynb](project_notebook.ipynb) - Jupyter Notebook 

## Technologies
* [Python](https://www.python.org/)
* [pandas](https://pandas.pydata.org/) library
* [matplotlib](https://matplotlib.org/) library
* [sqlite3](https://docs.python.org/3/library/sqlite3.html) library

## Methods
1. Clone this repo (for help see this [tutorial](https://help.github.com/articles/cloning-a-repository/)).
2. Gather and import [raw data](./zippedData)
3. Combine, join, and clean data
3. Exploratory Data Analysis to form recommendations
4. Plot visualizations

### The Data

#### Data Description

In the folder `zippedData` are movie datasets from:

* `bom.movie_gross.csv.gz`: [Box Office Mojo](https://www.boxofficemojo.com/)
	* stored in compressed CSV
	* contains domestic and foreign gross revenue
* `tn.movie_budget.csv.gz`: [The Numbers](https://www.the-numbers.com/)
	* stored in compressed cSV
	* contains production budget

Box Office Mojo and The Numbers data are stored in compressed CSV (comma-separated values).

* `im.db.zip`: [IMDB](https://www.imdb.com/)
	* stored in a SQLite database
	* contains user-generated rankings on a scale of 0 - 10 with 0 being the worse and 10 the best

## Data Analysis and Recommendations

### Movie genre does not have an effect on IMDb 
* More profitable movies do not on average much difference in user ranking

![IMDb Ranking by Movie Genre](./img/fig/barplot_genre_ranking.png)

###  Movie genre should be a combination of Action, Adventure, Animation, or Sci-Fi
* Generate the most worldwide gross revenue

![Average Revenue by Genre](./img/fig/barplot_genre_revenue.png)

###  The movie should be released in Q2 or Q4
* Q2 and Q4 have the highest revenue

![Revenue by quarterly release time](./img/fig/barplot_comp_quarter.png)

###  Expect to budget between $100 million per movie
* The highest revenue generators also have the highest production budgets

![Average Budget by Genre](./img/fig/barplot_genre_budget.png)

## Conclusions
* Summary of conclusions including three relevant findings

