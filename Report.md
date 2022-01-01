## Initial Training

### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?

I noticed an error in submitting the result. I revised the error in kaggle and it was mentioned that the datetime column was missing.



### What was the top ranked model that performed?

The top model was WeightedEnsemble_L3

## Exploratory data analysis and feature creation

### What did the exploratory analysis find and how did you add additional features?

In EDA I draw a histogram for all the features to know the type of distribution it follows. I found that "atemp","temp" and "humidity" feature almost folows normal distribution.

I splitted the datetime feature into hour, day, year and month.

### How much better did your model preform after adding additional features and why do you think that is?

TODO: After adding the additional features, the RMSE decreased from 1.39 to 0.47.

## Hyper parameter tuning

### How much better did your model preform after trying different hyper parameters?

After i changed the hyperparameters i found the RMSE increased a little bit, which means that the combination I chose was not better than the previous one.

### If you were given more time with this dataset, where do you think you would spend more time?

I would consider spending more time in data cleaning and transformation. Also I would consider searching for a way to find the best combination of hyperparamters to achieve a better result.

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.

| model        | Time_Limit | Verbosity | num_bag_folds | score |
|--------------|------|------|------|-------|
| initial      | 600  | 2    | None    |1.39275|
| add_features | 600  | 2    | None    |0.47102|
| hpo          | 100  | 1    | 7    |0.52935|

![model_test_score.png](data:C:\Users\inova-user\Downloads\nd189-1-Introduction-to-Machine-Learning-project-starter-main\nd189-1-Introduction-to-Machine-Learning-project-starter-main\project\img\model_train_score.png)

## Summary

In conclusion, I learned the impotance of featrue engineering and hyperparameter tuning and how the affect the final reasult of the model.
