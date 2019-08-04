<img align="center" width="200" height="200" src="./visuals/nba.png">

**Authors: Erin Hwang, Vala Rahmani**

# Hackathon Phase 1

## Objective:
Predict Instagram engagements using based on the following information: 
- `Followers at Posting` - (int)
    - Number of followers NBA official has at time of posting
- `Created` - (datetime)
    - Date and time of posting 
- `Type` - (object)
    - Type of post (photo, video, album)
- `Description` - (object)
    - Caption (includes tags and hashtags)
    

## Results
- Random Forest had the best overall train, test, and MAPE score when GridSearching for optimal paramters. 

Here is a table of our results when GridSearching for optimal parameters:

|Model|Train Score|Test Score|Mape Score|GridSearch Name|
|--|--|--|--|--|
|Lasso|.9638|.8736|8.749|gs2|
|Ridge|.9384|.8949|8.08|gs3|
|Random Forest|.988|.9127|**7.0428**|gs|
|Elastic Net|.963|.873|8.749|gs4|

**We decided to proceed with Random Forest Regressor**
