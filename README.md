a. Name: Stan
Surname: Eduard George
Link to Kaggle profile: https://www.kaggle.com/edystan
Username: Eduard Stan

b. Link to project: https://github.com/EdyStan/titanic_spaceship
EDA: https://github.com/EdyStan/titanic_spaceship/blob/main/EDA.ipynb
solution: https://github.com/EdyStan/titanic_spaceship/blob/main/solution.ipynb

c. After measuring performance for all models trained, I decided to stick with the Random Forest Classifier. A random forest model always leaves space for improvement, and I am absolutely sure that my solution can be improved even more, via various fine tune methods.

d. A great source of information that covers a large part of Machine Learning is the book "Hands-On Machine Learning with Scikit-Learn, Keras & TensorFlow" by Aurelien Geron. It strengthened my knowledge about ML, even though I am still in course of reading it. Other useful tutorials were found on YouTube, the majority of them from Tech with Tim channel.

In the first part of the project, I inspected some accessible attributes of the dataset via methods like: .info(), .describe(), but I also generated histograms and a heatmap of the correlation matrix of the dataset.
After I split the data into training and test sets, I created pipelines in order to transform data to its best form (filled the missing values, scaled the numerical attributes, encoded text typed categorical features, and separated them into more columns and finally encoded boolean values too).
Then, I chose 5 models: `linear regression`, `decision tree regressor`, `random forest regressor`, `logistic regression` and `random forest classifier`.
There were chosen such different algorithms (three for regression and two for classification) because there were no graphs showing any visible correlation between any feature and the label. One important hint was the presence of some boolean fields, inclusively the label, that led to choosing the `logistic regression`.
`Decision tree regressor` and `linear regression` are some of the most common models, so I decided to add them, mostly for comparison reasons.
Both `random forest` models were chosen because it is said that they are the best algorithms at this moment.
After training the selected models, I evaluated their performance using rmse and accuracy where needed.
After interpreting the results, I decided to stick with `Random forest classifier` and then I fine-tuned its hyperparameters, getting an even bigger accuracy.
Having the model ready, it was one more thing left: predicting the requested data.

A better explanation is found in the code files.

In the first instance, I chose the `random forest regressor` model and even fine-tuned it. Then, I realised that 0.38 is not really a small rmse, and, logically speaking, given the dataset (full of booleans), it was clear that a classification model would work better. And then I decided to use a classifier instead. 

Overall, this was a great exercise. I learned how to handle pipelines better and how to simplify my code and reduce it to a clean and totally readable one. I better understood fine tune of a model and how to graphically represent the relations between features.

Ideas of improving my solutions are making better graphic representations, better scaling, maybe on a log scale. Paying more attention over correlations between features, maybe by creating new features, combining two of more existing ones. Another idea would be training more models and combining them for a better result.
