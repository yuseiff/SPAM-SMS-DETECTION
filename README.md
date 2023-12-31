# SPAM-SMS-DETECTION

This project focuses on detecting spam SMS messages using a logistic regression model. The dataset used for training and evaluation contains SMS messages labeled as either "spam" or "ham" (non-spam). The goal is to build a model that can accurately classify new SMS messages as either spam or ham based on the content of the message.
The project begins by importing necessary libraries such as numpy, pandas, and scikit-learn. The dataset is loaded from a CSV file named 'spam.csv' using pandas' read_csv() function and stored in a DataFrame.
After loading the dataset, some initial exploration is performed. The shape and information of the dataset are checked to understand its size and the available columns. Unnecessary columns are dropped, and duplicated entries are examined and handled if present.
Further analysis is conducted by counting the occurrences of each label (spam or ham) in the dataset and visualizing the distribution using a count plot and a pie chart. This helps understand the class balance and the proportion of spam and ham messages in the dataset.
Next, the data is preprocessed to convert the text labels (spam and ham) into binary values (1 and 0) to make them suitable for training a machine learning model. The columns 'v1' and 'v2' are renamed to 'target' and 'Text', respectively, for clarity.
The data is then split into the target variable y_train (containing the binary labels) and the feature variable X_train (containing the text messages). To prepare the text data for modeling, feature extraction is performed using the TF-IDF vectorization technique. This transforms the text data into numerical features that can be used by the logistic regression model.
The target variable y_train is converted to integer type for compatibility with the logistic regression model. A logistic regression model is then trained using scikit-learn's LogisticRegression() class and its fit() method.
After training the model, its accuracy on the training data is evaluated using the accuracy_score() function from scikit-learn's metrics module. The accuracy score provides an indication of how well the model is performing in classifying the SMS messages as spam or ham.
Finally, the accuracy score on the training data is printed, which gives an understanding of the model's performance in the context of the training dataset.
Overall, this project demonstrates the process of building a logistic regression model for spam SMS detection, from data loading and preprocessing to training and evaluation.


Follow me on linkedin: https://www.linkedin.com/in/youssef-husseiny-989a17257/
