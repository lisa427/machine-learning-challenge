# machine-learning-challenge

The goal is to create a machine learning model that can classify exoplanets using data collected from NASA with at least an 85% accuracy.  NASA has a dataset that has been labeled with the classification of exoplanets gathered from the Kepler space telescope.  This dataset can be used to create a supervised machine learning model with a classification algorithm.  

The first model I created uses Logistic Regression.  It only scored 80% on the test data after being trained.  To attempt to better tune the model's parameters, GridSearch was used.  This resulted in 81%, but it wasn't yet at the goal.

The second model I created uses a Random Forest algorithm.  This model scored an 86% which meets the goal.  In order to try to create an even better model, I tuned the parameters using both RandomizedSearch and GridSearch.  Because Random Forest models have so many parameters, the RandomizedSearch is helpful to narrow down what ranges of parameters to use for the GridSearch.  The accuracy score ended up being the same, with the precision and recall scores being slightly worse.  I decided to save the original Random Forest model to a file to be used as the final model.

Both of these models use 15 features.  The next step would be experimenting with models that use less features and achieve the same (or better) results.  This would save processing time and possibly improve the model by decreasing the chance of overfitting.  Creating models using different classification algorithms could also improve the accuracy score.  