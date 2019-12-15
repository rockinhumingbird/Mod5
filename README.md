# Mod5
Youtube
## Goal
Build a classifier that predict category of a given yotube information to one of the following categories: 
Gaming/Sports, Entertainment, Films, Music, lifestyle and travel, STEM.

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
![header](Images/pca.png)
##
![header](Images/.png)

## Performance of ML Models
![header](Images/results.png)

## Precision and Call curve 
![header](Images/Precisionrecallcurve.png)
Although I checked for imbalanced problems, I want to show the accuracy of the model, effect size of the model using Precision and recall.
# Some feature imporance
![header](Images/featureimportance.png)

## Result
![header]let us go with the grid searched random forest with entropy criterion, max depth 5, it turns out, there is a strong indication on the role of number of likes, comments and length of the tags on the classifications of the video categories. 

