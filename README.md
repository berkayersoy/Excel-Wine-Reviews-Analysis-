# Excel Wine Reviews Analysis
Found a dataset on wine reviews, decided to do a fast ad-hoc style analysis on it with Excel to see if it returns some interesting insights.
The data set comes from kaggle by the author zackthoutt, the initial dataset can be found here: https://www.kaggle.com/datasets/zynicide/wine-reviews

My initial questions that I wanted to answer from this data set were:
1) Is there a correlation between wine price and rating ?
2) Which price range gives us the top rated wines with least bucks ?
3) Where are my personal favorite wine varieties (Merlot and Cabernet Sauvignon) rated in the scale ?

So the dataset was in csv format so I easily loaded into my excel sheet. Since this is going to be an ad-hoc analysis fast pivot table creation and looking for insights, I didn't see the use of formatting the data as a table and dived into the creation of the pivot table and charts.


![1-what_the_data_initally_looked_like](https://user-images.githubusercontent.com/44724944/197541292-3b6456f2-9d14-4a57-b98e-f06420f4467d.png)
<p align="center">
This is how the data looked, the columns that I was interested in from dimensions was the name of the variety and from measures it was the price and also the rating of the wines.
</p>


![2-wine_variety_average_ratings_without_threshold_filter](https://user-images.githubusercontent.com/44724944/197541309-9aafc93b-77a5-45f3-89aa-17e1058acd8f.png)
<p align="center">
Then I inserted the pivot table with Variety as rows, average rating and count of reviews as columns.
</p>


![2-2-average_points_by_variety](https://user-images.githubusercontent.com/44724944/197541320-f4761975-24be-4c3f-b94e-10dc1db1d4b6.png)
<p align="center">
I filtered out the noise and just kept the wines that only had more than 300 reviews for a more accurate result. At this point I could easily see the answer of my third question, Cabernet Sauvignon had average rating of 88.6 and Merlot a bit lower rated at 87.2 compared to others in the list.
</p>


![3-wine_price_rating_pivot_chart](https://user-images.githubusercontent.com/44724944/197541333-8b49bf30-8906-49b9-81c9-b3c5d8f226e3.png)
<p align="center">
I quickly created a pivot chart price against rating to see if there is a trendline and a sweet spot to buy highly rated wined at a good price. On this chart we can see between roughly 70 to 130 dolars we can get a high rated wine.
</p>

![4_added_a_logarithmic_trendline_and_scaled](https://user-images.githubusercontent.com/44724944/197541341-6cae9f6f-a48a-44e5-8dbc-4268bef93db7.png)
<p align="center">
To observe the trend a bit easier I added a logarithmic trendline.
</p>


![5-grouped_values](https://user-images.githubusercontent.com/44724944/197541372-808c87d0-cd10-4e97-945d-e5d0c7b8a44c.png)
<p align="center">
At last I grouped up the values to further analyze the trend. To answer my questions 1 and 2 I asked to myself in the beginning when I was starting this analysis, we can clearly conclude by stating that there is a corralation between wine price and rating upto a certain price (70-150 usd) but then the trendline becomes flat. 100-150 usd price range seems like the sweet spot for getting yourself a high rated wine for a good price!
</p>
