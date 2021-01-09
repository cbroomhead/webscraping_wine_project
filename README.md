[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/cbroomhead/webscraping_wine_project.git/main)

.. image:: https://mybinder.org/badge_logo.svg
 :target: https://mybinder.org/v2/gh/cbroomhead/webscraping_wine_project.git/main

# wine.com webscraping project 

## Included


## Run
To view the results of the analsyis, open this '' in a browser. 
If you wish to run the actual webscraping tool, collecting the data might take upwards of two hours. 


## Introduction
The project was to learn how to use a webscraping tool and analyse the dataset. The webiste scraped is wine.com's 'Best Rated Wines Online 94 Points &amp; Above| Wine.com'.
The dataset contains +23,822 rows and wine attributes such as: product name, retail price, varietal, origin, average rating, and count of ratings. 
After cleaning the dataset I ended up with 22,579 entries. 


## Project Tools
Tools used in the gathering portion of project: Python, pandas, Beautiful Soup 4, requests, and os. 
Tools used in the analysing portion of project: Python, pandas, statsmodels, and matplotlib. 
Tools used in the visualization portion of project: Python, pandas, seaborn, and nbconvert. 


## Project Questions

Basic / Assess
- Top high rated wines?
- Which varietals tend to get the highest ratings? Conversly, which varietals have low ratings?
- Which appelation tend to get he highest ratings? Conversly, which appellation have low ratings?
- Where are the most expensive wines from? Conversely the cheapest wines?
- Which are some of the most popular varieties and from where?

 
Realtionships / Analyze
- Do higher rating counts mean higher average rating?
- Does price correlate with high ratings?
- Does year correlate with high ratings?
Does year correlate with regions or appelation?
Does price correlate with regions or appelation?


Report Write up:
Which wines are the best bang for the buck according to the ratings?
What are wines I should generally stay away from according to the ratings?
When considering a cheaper wine, which region and appelation should I get?
When considering a cheaper wine, which varietals should I consider?
-> There might be a bias in the data since there were a lot of California wines and most people who rated the wines were from within the US. 

Deep dive into California wines:
- Which CA wines have the highest ratings?
- How does year affect the ratings of the wine? Are there years to stay away from?
- How does price affect the ratings of the wine?

Predictive:
Target vector could be rating, rating_count and price. 

Feature Engineering:
red, white, or sparkling?
import precipitation data to see if there is correlation with price or ratings



### Oldest Wine
1) Filtering out for the year. The product info in the web pages did not contain a seperate field for the vintage year. Instead, the year was part of the product_name so it was pretty painful to extract the date string out the product name. After several attempts I ended up with an approach that minimized the amount of string that I had to drop due to improper dates being extracted. The oldest wine listed on the web page filter was 1982 so I chose that date as my cutofff. 

## Citations
wine.com