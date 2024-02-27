# CODSOFT-TASK-1
# MOVIE-GENRE-CLASSIFICATION
## Import Libraries:

Import necessary libraries such as pandas, matplotlib, seaborn, nltk, string, and relevant modules from sklearn.
## Load Training Data:

Read the training data from a file (train_data.txt) into a Pandas DataFrame. The data contains columns 'Title', 'Genre', and 'Description'.
## Data Exploration:

Use describe(), info(), and isnull().sum() to get a summary, information, and check for null values in the training data.
## Load Test Data:

Read the test data from a file (test_data.txt) into another Pandas DataFrame. This data has columns 'Id', 'Title', and 'Description'.
## Genre Distribution Visualization:

Plot the distribution of genres in the training data using both a count plot and a bar plot.
## Text Cleaning:

Define a function clean_text to preprocess the text data. It converts text to lowercase, removes Twitter handles, URLs, non-alphabetic characters, stopwords, and extra spaces. This function is then applied to the 'Description' column in both training and test datasets.
## Text Length Visualization:

Calculate the length of the cleaned text and visualize its distribution in a histogram.
## TF-IDF Vectorization:

Use TfidfVectorizer to convert the cleaned text data into a TF-IDF representation. Fit and transform the training data, and transform the test data accordingly.
## Train-Validation Split:

Split the training data into training and validation sets using train_test_split.
## Multinomial Naive Bayes Classification:

Initialize a Multinomial Naive Bayes classifier, fit it to the training data, and make predictions on the validation set.
### Model Evaluation:
Evaluate the performance of the model on the validation set using accuracy and classification report.
### Make Predictions on Test Data:
Use the trained model to predict genres for the test data.
### Save Predictions to CSV:
Save the test data DataFrame with predicted genres to a CSV file named 'predicted_genres.csv'.
### Display Predicted Genres:
Print the test data DataFrame with predicted genres.
The code essentially performs text preprocessing, vectorization, model training, and prediction for movie genre classification. The final predicted genres for the test data are saved in a CSV file named 'predicted_genres.csv'.




