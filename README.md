Overview-

Student Feedback Sentiment Analyser is created in Django, for frontend we used Bootstrap and backend is handled by Python.

This tool is working on a naive bayes algorithm, we use MultinomialNB (Multinomial Naive Bayes) from sklearn python library.

We trained our algorithm by passing student feedback dataset, which contain feedback comment and its points(0,1,-1).

0 for neutral comment
1 for positive comment
-1 for negative comment

Working-

First we are taking input from excel sheet (feedback comment and points) with the help of python pandas library, then we are cleaning that data before test and train. We used CountVectorizer to tokenize sentences and also remove stopwords to clean data, finally we divided test and train data with the test size 0.3 to create classifier using MultinomialNB.

We use this trained classifier to predict the output and generate report using classification_metric from sklearn, Finally we got accuracy of 79%

To show data insights we use confusion matrix, wordcloud, Pie Chart, Classification Report.

Student can also give feedback on this platform, that feedback will be added in existing dataset that will be further use for analysis.

Set-up-

1. Clone the project.
2. Download the required libraries mentioned in the requirement.txt file.
3. Make migrations and migrate them.
4. Create a superuser and run the server.
5. The web app will start working.
