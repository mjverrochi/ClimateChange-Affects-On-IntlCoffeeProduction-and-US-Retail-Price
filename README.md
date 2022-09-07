# Goal 
The goal of this project is to collect data from Reddit by scraping the website and building a binary predictor. It is intended to help Nate Silver and co. at FiveThirtyEight to determine what may or may not affect a Reddit post's popularity (measured by number of comments).
After scraping, cleaning, and conducting exploritory data analysis I will create a random forest classifier and logistic regression to analize findings.
Sucess will be determined by metric scores.

# Summary
This report aims to predict whether or not a given Reddit post will have above or below the median number of comments.


Data Dictionary of Features Used

|Feature|Type|Dataset|Description|
|---|---|---|---|
|title|object|df|title of reddit post|
|subreddit|object||df|subreddit that the post belongs to|
|subscribers|int64|df|number of subscribers that the poster has|
|created|object|df|when the post was made|
|over_18|int64|df|whether or not the post is tagged as "over 18"/"NSFW"|
|spoiler|int64|df|whether or not the post is tagged as containing spoilers|
|is_video|int64|df|whether or not the post has contains a video|
|abv_median|int64|df|whether or not the number of post comments is above the median for the dataset|


Data Observations
Data is from 8/2012 - 9/2022.

Interpretation of Model
Both our random trees classifier and extra trees classifier result in about a 56% accuracy rate of our dataset items. Our logistic regression
scores (90% train, 58% test) show us that our model is overfit. Further analysis and feature engineering is to be done be decrease that overfit.
Our precision, recall, and f1 scores are all above 50%. Hoping to improve that with the increased feature engineering.


What Next
Things I would like to look into as the project continues:
I would like to continue feature engineering to increase scores and metrics.
Features inparticular are over_18, spoiler, is_video.

Conclusions and Recomendations
Be mindful of what title is used to post as it does appear to have an affect on comments received
Having a title/post relating to Time may increase chance of post popularity
Analyzing title alone predicts better than our baseline

