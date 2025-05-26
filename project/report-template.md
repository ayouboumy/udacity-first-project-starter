# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### AYOUB HANFOURI

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
TODO: When i was going to submit my first prediction using the initial data and the hyperparameters, we i found some negative results in the prediction output, so to have a valide submition i replaced the negatives values to zero (since the negative values mean no count)

### What was the top ranked model that performed?
TODO: the top ranked model was the first hyperparameters tuned model where i used the GBM and the XGB model types

## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
TODO: i found that season and weather features have distinct values so i turned their types to categorical, and i did add hour and day features extracted from datetime feature
### How much better did your model preform after adding additional features and why do you think that is?
TODO: the first score was 1.84461 and after adding the does new features it goes to 0.62687 which is better, i think that the model worked better because the introducing of the hour and day features makes the model get some patterns and understands the renting hours and days which can help it exclude the holidays and the night hours where the renting is down.

## Hyper parameter tuning
### How much better did your model preform after trying different hyper parameters?
TODO: it get better and the best ranking score was 0.51743

### If you were given more time with this dataset, where do you think you would spend more time?
TODO: in the data engineering and scaling i think, normalize some and try to make some features combinations and add some new ones

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|
|--|--|--|--|--|
|initial|None|None|None|1.84461|
|add_features|None|None|None|0.62687|
|hpo|"model type = 'GBM' , 'XGB'"|"num_bag_folds=5,num_bag_sets=10, num_stack_levels=1"|"auto_stack = True"|0.51743|

### Create a line plot showing the top model score for the three (or more) training runs during the project.

TODO: Replace the image below with your own.

![model_train_score](<training score.png>)

### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

TODO: Replace the image below with your own.

![model_test_score.png](<test score.png>)
## Summary
TODO: during this project i could put the knowledge gained in the nanodegree classes into practice, from data exploration, model fitting to model tuning, we can notice the a new feature can make the model work more better, hyperparamters tunning play an other work progress to.
