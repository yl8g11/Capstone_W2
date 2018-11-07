## Welcome to My IBM Capstone Project Pages

In this capstone project, we try to detect the most overrated and underrated restaurants around a place (by default, we choose the location: North York, ON). 

We use the [Foursquare](https://developer.foursquare.com/) API to extract the venue IDs of recommended restaurants in North York and then get details of each restaurant, including price, the count of likes, and their ratings.

We then fit our multiple linear regression model: rating = 6.18032919 + 0.39078905 x price + 0.00811921 x likes.

With the model we can estimate the predicted rating for each restaurant. A restaurant is classified as overrated if its actual rating is higher than its predicted rating, and deemed as underrated if actual rating is lower than predicted rating.

### Most Overrated Restaurants

name | category |	address	| postalcode	| lat	| lng	| rating | predicted rating | difference
---- | -------- | ------- | ----------- | --- | --- | ------ | ---------------- | ----------
Buk Chang Dong Soon Tofu 북창동 순두부 돌솥밥 | Korean Restaurant | 5445 Yonge St. | M2N 5S1 | 43.777219 | -79.414861 | 8.4 | 7.4 | 1.0
MYMY Chicken | Fried Chicken Joint | 9 Spring Garden Ave | M2N 3G1 | 43.764658 | -79.411096 | 7.7 | 6.7 | 1.0
Aroma Espresso Bar | Café | 6 Parkhome | NaN | 43.769449 | -79.413081 | 7.5 | 6.7 | 0.8
The Fry | Fried Chicken Joint | 4864 Yonge Street | M2N 5N2 | 43.762993 | -79.411442 | 7.4 | 6.7 | 0.7
Pizzaiolo | Pizza Place | 4920 Yonge St. | M2N 5N5 | 43.764289 | -79.411780 | 7.3 | 6.6 | 0.7

### Most Underrated Restaurants

name | category |	address	| postalcode	| lat	| lng	| rating | predicted rating | difference
---- | -------- | ------- | ----------- | --- | --- | ------ | ---------------- | ----------
Oh Geul Boh Geul 오글보글 | Korean Restaurant | 5320 Yonge St	| M2N 5P9	| 43.773151	| -79.413915 | 6.1 | 7.2 | -1.1
Jack Astor's Bar & Grill | Restaurant | 5051 Yonge St | M2N 5P2 | 43.767097 | -79.412263 | 7.1 | 8.1 | -1.0
Bar Koyoi	Japanese Restaurant | 5347 Yonge St | M2N 7A1 | 43.774943 | -79.414306 | 6.3 | 7.0 | -0.7
Pho 88 Vietnamese Cuisine | Vietnamese Restaurant | 5197 Yonge St | NaN | 43.770456 | -79.413064 | 6.6 | 7.2 | -0.6
Kiyomizu Japanese Restaurant | Japanese Restaurant | 41 Spring Garden Ave. | NaN | 43.764820 | -79.410106 | 6.5 | 7.1 | -0.6

### Leaflet Map

We plot the above mentioned restaurants on leaflet map, with blue circles representing overrated restaurants and red circles representing underrated restaurants.

![over_under_rated](https://user-images.githubusercontent.com/43836620/48100994-79b4e180-e1f3-11e8-998a-25e5f38479f1.JPG)

### Notebook

My Python 3 code for this capstone project is available at [Cap_W2_Notebook.ipynb](https://github.com/yl8g11/Capstone_W2/blob/master/Cap_W2_Notebook.ipynb). 

### Report

For a full report of my project, you can click on [Cap_W2_Report.ipynb](https://github.com/yl8g11/Capstone_W2/blob/master/Cap_W2_Report.ipynb). 

### Help on Hosting Your Website on Github

You can view the source of this Markdown in the repository's `README.md` file.

For more details of how to use Markdown to create your website, see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/). If you have trouble with pages, you can check out github [documentation](https://help.github.com/categories/github-pages-basics/).
