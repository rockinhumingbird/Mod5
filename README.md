# Mod5
youtube

![header](Images/youtube.png)

## Goal
Build a classifier that predict category of a given yotube information to one of the following categories: 

## Data Cleaning
- A list of titles, classified (Kaggle). We extracted the 21 subreddits EACH classified as ‘arts’ and as ‘programming’ -- balanced data!
- The .tsv file can be found here: https://www.kaggle.com/mswarbrickjones/reddit-selfposts#subreddit_info.csv
- 1,000 reddit posts from every subreddit - we pulled 42,000 posts from our 42 subreddits

## Variables
- Classification goal: video categories:
- number of total likes
- number of total dislikes
- number of views
- number of comments
- length of the video title per word
- number of tags

- Qualitative: title words, tag words


## Data Preprocessing / Feature Engineering
for title We used NLTK to tokenize, lemmatize and filter the data, giving us 4000 unique features (words). From there we vectorized the data via TF-IDF calculation and dropped words below a threshold of 0.001. 
This left us with around 354 words to model!

## Visualization of Data in Reduced Dimensions
![header](Images/2d.png)

![header](Images/3d.png)

## Performance of ML Models
![header](Images/evaluation.png)

## Result
![header](Images/mnb.png)

