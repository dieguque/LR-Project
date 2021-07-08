# Minimum Viable Product (MVP)

## What factors predict the global success of a movie?

Analizing differents quantitative features like Budget, Worldwide Gross, Domestic Gross, Running Time, and Wide Release. We created a model to see which factors affects on the global succes of a movie.

![](https://github.com/dieguque/Movies_Project/blob/2378c360866f1caeba751af20be725dfdec66e50/MVP/charts/pairplot.png)

On this heat map we can how higly correlated Domestic Gross (0.94) and Opening (0.9) are to Worldwide Gross.

![](https://github.com/dieguque/Movies_Project/blob/2378c360866f1caeba751af20be725dfdec66e50/MVP/charts/big_heat_map.png)

### Baseline Linear Regression of R^2 = 0.91

This mean our model is trying to precit and not to describe or analyze. So let's remove Domestic Gross and Opening.

![](https://github.com/dieguque/Movies_Project/blob/2378c360866f1caeba751af20be725dfdec66e50/MVP/charts/pairplot_small.png)

And this is our smaller heatmap:

![](https://github.com/dieguque/Movies_Project/blob/2378c360866f1caeba751af20be725dfdec66e50/MVP/charts/small_heat_map.png)

### Baseline Linear Regresion of R^2 = 0.58

These feature improves our predective model and the next steps is to add the categorical data like Genres, MTAA Rating, Distributor and the Release Season.
