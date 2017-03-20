------ Rossmann Forecast --------

To run the code, please make sure the train.csv, test.csv, store.csv, and submission-sample.csv data sets from the Kaggle website (https://www.kaggle.com/c/rossmann-store-sales/data) are in the same folder as the IPyNB. After this, the whole thing can be run in one go with the output being poly3.csv which is a file with 41,088 lines in the format specified in submission-sample.csv.

In this challenge, the task was to predict the sales values for individual Rossmann stores (1,115) for a period of 6 weeks. A training set was given for 2 years with an additional data set with extra store information.

By exploring the data using various plots and graphics in matplotlib and seaborn, I discovered several trends and features which I thought to have significant correlation to the final sales values. The process is documented in-line in the notebook. Based on these visualizations I selected my features and prepared them to be run in a linear regression. A key trend I decided to focus on is a third-degree polynomial fitting of the data within the relevant timeframe (Aug.1 - Sept. 17), after fitting the data with this polynomial, I saw an increase in fit of the data when running linear regression.
