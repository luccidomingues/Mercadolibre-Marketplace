# Mercadolibre-Marketplace

Description:
In the context of Mercadolibre's Marketplace an algorithm is needed to predict if an item listed in the marketplace is new or used.

My task involves the data analysis, designing, processing and modeling of a machine learning solution to predict if an item is new or used and then evaluate the model over held-out test data.

To assist in that task a dataset is provided in `MLA_100k_checked_v3.jsonlines` and a function `build_dataset` to read that dataset in `new_or_used.py`.


Above an explanation on the criteria applied to choose the features, the proposed metrics and the performance achieved on that metrics.

The chosen model was the Gradient Boosting Classifier with an accuracy of 86.20% (using an approach based on feature selection using the RFE method and
by selecting hyperparameters using the GridSearchCV method). I covered 9 different classification models in the project, including models from different groups
such as: ensemble, naive bayes, svm, neural network, linear model and tree. 
I think you can explore many paths, settings, selections and parameters in this design journey with classification models, I highlight the Decision Tree models,
Random Forest, AdaBoost and Extra Tree. The performance and performance of these models they were very relevant.

I would like to propose the accuracy metric (it had 88%) as the second metric of the proposed exercise, I think that the proposed problem is related to the route of
customer purchase, so I guess we could try to reduce the amount of fake positives, leading the client to a lesser sense of frustration. When the false positives, increases accuracy. In the average point of view, it is preferable that the client has a new product thinking that it is used than on the contrary, a used one thinking it's new.

For feature selection, I used the RFE method from the feature selection library Scikit Learn features, as well as analyze and explore the features through filters in
plotted tables and graphs.

For the next steps, I would propose a better structure of the solution and some functions that are very reusable for models. As an example of functions for
select features and functions to select hyperparameters as well I would propose the creation of an application for the deployment of the solution. As
suggestion I propose the App Streamlit.

In the project he used the CRISP methodology for the development and approach of projects of Data Science. Evaluates the journey based on constant cycles and iterations with data, with analysis, business understanding, data preparation, analysis and modeling, validation and deployment.
