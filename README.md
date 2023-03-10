### What to eat? Ordering in (Glovo) or eating out (TripAdvisor)

![image](https://user-images.githubusercontent.com/121023453/216971838-8f1c6669-f68d-4f91-95a3-8d3295ca4836.png)

We want to find out to what kind of restaurant we should go to or order from. 

We found a TripAdvisor dataset on Kaggle with data of 125000 restaurants in Europe (https://www.kaggle.com/datasets/damienbeneschi/krakow-ta-restaurans-data-raw), first we cleaned the data by removing restaurants in all cities other than Barcelona, removing columns we don't need and we ended up with a dataframe of 8425 restaurants in Barcelona with name, cuisine style, the rating and amount of reviews. 

To get similar data from Glovo, we used data scraping. By using data scraping we got the restaurant name, cuisine style, rating and amount of reviews from 1516 restaurants in Barcelona.

When merging those columns by name we only had about 110 exact matches, then I went back to the dataset and figured that the dataset was uploaded over 5 years ago. For that reason we decided to also use webscraping for TripAdvisor instead of using this dataset. By doing that we got the same information from 9700 restaurants in Barcelona.


![image](https://user-images.githubusercontent.com/121023453/216971245-16de2863-253f-4a7a-bc55-8b3d9c4fda98.png)


Here we see the most common types of food offered on both platforms, we can see that for odering food people prefer fast food as Pizza and burgers, while for eating out Mediterranean and Japanese are the most common. 


![image](https://user-images.githubusercontent.com/121023453/216972268-fe337714-e638-41d1-bfb5-b30b0888f020.png)


An overview of the categories with the highest ratings on Glovo and TripAdvisor. There is a big difference between the cuisines in both charts, probably because in Glovo after every order you get a pop-up screen asking for a thumbs up/thumbs down for every order and people are easily satisfied with a breakfast, brunch, bakery items etc. While in TripAdvisor people have to be proactive to leave a review after their visit. 


![image](https://user-images.githubusercontent.com/121023453/216974285-4532cfc5-186a-4d73-aeb2-4a4c907d33ed.png)

And the lowest rated cuisines

![image](https://user-images.githubusercontent.com/121023453/216980456-f09786b0-629a-48d2-b3a8-e10847b32078.png)
In the boxplots above we see that the rating of restaurants in Glovo is higher than in TripAdvisor. Which might also be affected by the way Glovo asks for a thumbs up/thumbs down once you open the app again after ordering. 

![image](https://user-images.githubusercontent.com/121023453/217066802-22780862-444e-468a-b840-7705e1dde5c7.png)

In the bubble plot above we see the cuisines by average rating and the size of the bubble indicates the amount of reviews it has


![image](https://user-images.githubusercontent.com/121023453/217068261-7bb52752-a4b7-4a6e-b7a7-d50fcd062d33.png)

TripAdvisor has a lot more different types of Cuisines, so we devided it in 2 charts 


![image](https://user-images.githubusercontent.com/121023453/217073148-e6f6175b-015e-43ac-ae17-0acf6d2fb025.png)


A chart of cuisines of all nationalities in class (Pub = English)

![image](https://user-images.githubusercontent.com/121023453/216987376-4fba2e1a-36aa-42f1-b4fb-dbfdcc703036.png)

When merging both dataframes to one, with only showing restaurants that are on both platforms we have a dataframe of 355 restaurants. The avarage score of those restaurants is 10% higher on Glovo than on TripAdvisor

### Conclusion

At the end we can conclude that: 
- People that leave a review on Glovo are about 10% more positive than people on TripAdvisor; even when it is about the same restaurant. This might have to do with the way the Glovo app is asking for a review (thumb up/thumb down) when you open the app once you received your food. While for TripAdvisor you have to actively leave a review.
- The more reviews the more difficult it is to have a high average score 
- Most restaurants that deliver food deliver Pizza or Burgers, while when it comes to going out for dinner most restaurants serve Medeterranian dishes. Sushi/Japanese however, is very popular for both. 
- With getting breakfast or brunch delivered you can't go wrong; those two categories have the highest rating of all on Glovo.
- When going out for Dinner in Barcelona you should go to Polish restaurant it has an average of 100% on TripAdvisor (based on low amount of reviews). When looking at cuisines with more reviews Japanese is the highest rated. 
- Avoid Kebab/Turkish restaurants to go to or order from, this is the only cuisine that is in the list of worst scoring cuisines in both lists.
