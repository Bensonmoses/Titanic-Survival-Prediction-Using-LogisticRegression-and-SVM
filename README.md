# Titanic-Survival-Prediction-Using-LogisticRegression-and-SVM

In this Titanic dataset project, we began by importing essential libraries like Pandas, NumPy, Seaborn, and Matplotlib. Then, we loaded the training and test datasets into Pandas DataFrames to explore and analyze the data.

Exploratory Data Analysis (EDA) was our first step, visualizing missing data using Seaborn's heatmap. We examined the "Survived" variable distribution with a histogram, breaking it down by gender. We also created a histogram to analyze passenger class distribution.

Data cleaning involved filling missing values for the "Age" column with the mean age, dropping the "Cabin," "Name," and "Ticket" columns, and removing rows with missing "Embarked" values. We applied these steps to both training and test datasets.

To prepare for modeling, we converted categorical features into numerical using Pandas' get_dummies method. We also dropped redundant features, such as "Sex_female."

For modeling, we trained a Logistic Regression model and a Support Vector Machine (SVM) model. We split the data, evaluated both models, and found the Logistic Regression model achieved around 81% accuracy, similar to the SVM model.

We fine-tuned the SVM model with GridSearch, finding optimal "C" and "gamma" values ("C=1" and "gamma=0.001").

Finally, we tested both models on the test dataset, generating predictions. Logistic Regression predicted 156 survivors, while SVM predicted 57.

In conclusion, Logistic Regression slightly outperformed SVM in accuracy. However, model choice may depend on other factors like interpretability and resources, considering specific problem goals and constraints.
