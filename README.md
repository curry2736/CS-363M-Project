<!-- ABOUT THE PROJECT -->

## About The Project

In this project, we used a dataset containing ex-college football players' game
stats and the round and pick in which they were drafted. After cleaning and
feature engineering the data, we trained a variety of models to predict what
round a player would get drafted at in the NFL draft based on their attributes
and statistics.

A significant amount of data cleaning and feature engineering was needed for
this. The data set had many NaN values that needed to be imputed in different
ways depending on the feature. In addition, there were many features that were
unneeded or provided information from the future. In order to have the best data
for our models, we decided to remove these. While future information would have
greatly improved the accuracy of our models, real-world data on college NFL
stats does not have things like their future team if they have not yet been
drafted. Next, we had to change the class labels from numbers into bins. With
the number of rounds we have, it is not feasible with the amount of time or
expertise we have to create a model that has good accuracy on 11+ classes. So,
we decided to bin the classes into 3 bins. This allows for our models to have a
higher accuracy as they don't need to be extremely precise. Finally, we also had
to change the number of classes (rounds) as prior to 1993, there were a
different number of rounds per pick. Thus, we had to standardize the data to
today's standard of 32 picks per round and 7 rounds per draft.

All of our models except for Naive Bayes had around the same accuracy (50-56%).
However, the highest was SVC at 0.56. We can compare this to the rate of
guessing randomly, which will give you a 33% accuracy rate. So, our best model
gives a 169% increase over randomly guessing.

The amount of time we spent data cleaning made up the majority of our work,
which was reflective of what a lot of data scientists do on the job. At the same
time, we think the majority of our models would be good to gain insights about
future drafts, assuming that our stakeholders are okay with the classes being
put into bins.
