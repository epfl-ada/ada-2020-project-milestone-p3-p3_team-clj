# Project milestone 3 : creative extension

## Predicting betrayals in movies

### Abstract
In this project, we want to extend the work of the 'Linguistic harbingers of betrayal' study to another dataset, in another context. We train a model that will predict a betrayal in a relationship, using the dataset from the paper; then test this model on dialogues from famous movies in which a character betrays another and see if the results of the paper apply to movies, or if not, what makes the difference. Betrayals in movies often, if not always, surprise the "victim" character(s), but also the spectator. If the model performs well on the movie scripts, it would be an indicator that it may be relevant to use in other contexts ; if not, it would highlight the difference between a purely textual exchange as in the Diplomacy game, and a more complex situation, including body language, intonations and facial expressions.

### Research Questions
- How different are movie dialogues from Diplomacy messages ?
- Can we train a classifier on a given dataset and obtain relevant results with it on a contextually different dataset ?
- Can we predict betrayal in movies from the lines of the potential betrayer ?

### Proposed dataset
- Dataset from the paper : we use it to train the model, using features from the betrayers' messages.
- Movie scripts (The Lion King, Interstellar, Matrix, Star Wars) : we get from internet, as .txt. We select dialogues between the betrayer and the victim before the betrayal happens, and extract the "messages" from the betrayer, then process the "messages" to obtain the same features used in the model (e.g. politeness score, positivity, etc. depending on which features are selected for the model).

### Methods
Internal milestones :
1) Finding the data : get the movie scripts, extract the relevant lines
2) Training the model : choose a classification method, select features, train and validate the model on the data from the paper
3) Processing the new data : extract the appropriate features and prepare a dataframe
4) Testing the model : use the model to predict betrayals with the new data and evaluate results
5) Report : prepare figures and write report or data story
6) Video : write and make the presentation video

Timeline :
27/11 to 04/12 : milestones 1 and 2
04/12 to 11/12 : milestones 3 and 4
11/12 to 18/12 : milestones 5 and 6
(add sketch + qui fait quoi)

### Questions for TAs (optional)
We think doing this project with movie scripts would be really interesting and a lot of fun, but maybe it's too complicated and ambitious, in which case, we thought about a "backup" project. Using the dataset from the paper, we could do an exploratory data analysis, looking at the distribution of the different features among the population of betrayers to see if there are different "profiles" of betrayers, and use a clustering method on the messages (maybe do a PCA then use k-means) to try to find different message types, and if certain types are mostly sent by betrayers. 
