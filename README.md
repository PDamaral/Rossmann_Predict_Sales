# Rossmann_Predict_Sales
Sales forecast for 6 weeks for several stores of the European pharmaceutical chain Rossmann - Timeseries Supervised regression (EN)

## Objective
Forecast for the next 6 weeks sales individually for each store in the company

## Developmento summary
Unifying the provided databases (sales data and store data), I performed the initial exploratory analysis, verifying null values (NAs) and applying different strategies, according to each feature, to fill them. Exploring numerical and categorical data, we can better understand the data and associate them with the business problem, in sequence, a hypothesis map is created, so that it is possible to validate the hypotheses and perform the feature engineering and univariate and bivariate analysis, where we validate the hypotheses.
After studying the data and the answers to the hypotheses, some insights can be generated at this point in the project, and the process of preparing the data (encoding) for machine learning begins. With the data adjusted and the selection of features made, in this case we use a specific library for this but we can also make comparisons of the best features coming from the exploratory analysis.
With the features selected, the data processed and possible to start the application of machine learning, initially we use a base value to be able to measure the progress of our models, the base value and just a simple statistical test like the average in this case. We applied 4 machine learning models (Linear regression , Lasso, Random Forest and XGBoost Regressor) using cross validation (testing each model 5 times considering the mean of the results) and MAE, MAPE and RMSE values as validation metrics.
In comparison, the chosen model was the XGBoost due to its speed and accuracy, using finetuning of the values for a better fit of the model.
With the model adjusted and applied to the database, we have the study of the error interpretation and the business performance of the model.
As a deployment method, the Pyckle library and the Heroku server were used to create a bot on Telegram so that the directors and managers of each store can access and have the sales forecast quickly and easily.*under development

## Conclusion
In this project, several data manipulation techniques, business concepts, libraries and machine learning are applied, being very complete, going through the full cycle of the CRISP methodology.
Even though the project was very focused on data development and on the best response, the business was never left aside, I always try to guide decisions on the use of resources (machine learning and model finetuning options) and business logic (completion of NAs according to functionality and comparison with existing data from other similar features). In addition to the deployment model chosen for covering a specific audience and with little time to be accessed (Management, board and C level).
From the business point of view, the more accurate the prediction of the model, the more strategic the decision-making can be, such as creating a budget for promotions and/or renovations or reducing/suspension of stores with low results. Also considering the insights session, we can break certain paradigms, such as the greater the stock, the greater the sales or times that sell more, as well as supporting strategic decisions.

