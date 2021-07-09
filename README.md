# Movie Suggestion for Movie Studio
Diego Duque

## Abstract
The goal of this project is to see if it is possible to predict the success of a movie and which factors affect the success of a movie using public data. The [Box Office Mojo](https://www.boxofficemojo.com) website was used to get the data through scraping. I used Python BeautyfulSoup for the whole scraping process and other packages for the modeling.

## Design
A hypothetical situation was created where a new movie studio asked us to see if it possible to predict the success of a movie and what are the key factors that make it possible. Consequently, I was approached to assume the Data Science consultant role. The client explicitly asked to use the [Box Office Mojo](https://www.boxofficemojo.com) website and present the results.

## Data
The data scraped includes all the movies from 2010 to 2019. This data was scraped using BeautyfulSoup which is an efficient package to scrape multiple websites using Python algorithms. In total 2000 movies were scraped and 1151 used after cleaning the data.

## Algorithms
*Scraping*:
The open-source software Jupyter Notebook was used running Python tools to clean, aggregate, and visualize the data.

*Modeling*:
Linear Regression (OLS) was used to analyze the numerical values: Budget, Widest Release and Runtime (in minutes):
  R^2 = 0.587.
### OLS (numerical values)
<img src="https://github.com/dieguque/Movies_Project/blob/8894bba9708f39c6f119e8d86d63969902eb2633/charts/OLS_num.png" >
  
Polynomial Regression was also used to improve our baseline model:
  R^2 = 0.756

Later, *Feature Engineering* was used to add the qualitative data like Season, Distributor, MPAA Rating, and Genres. Here the OLS with the qualitative was 
  R^2 = 0.882 

During this featured engineering **Ridge CV** was used:
  R^2 = 0.896
  
### Ridge CV
<img src="https://github.com/dieguque/Movies_Project/blob/1c7cabb094fc652e908c4d246719a2a6cb79ee70/charts/movies_ridge_log_jointplot.png" >
  
Also we used **LASSO CV** :  
  R^2 = 0.894
### LASSO CV
<img src="https://github.com/dieguque/Movies_Project/blob/1c7cabb094fc652e908c4d246719a2a6cb79ee70/charts/movies_lasso_log_jointplot.png" >


## Tools
  - BeautyfulSoup for scraping.
  - Sklearn to model.
  - Pandas, Datetime, and Numpy for data manipulation.
  - Matplotlib, Seaborn, Numpy, and StatsModels for plotting.

## Communication
By using [this link provided](https://github.com/dieguque/Movies_Project/blob/8894bba9708f39c6f119e8d86d63969902eb2633/movies_presentation.pdf), the slides used during the presentation may be accessed. On the chart below, I have summarized the project findings.




