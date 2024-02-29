Consumer Complaint classification means identifying the category of complaint. We use Machine Learning models to categorize the complaints based on product., NLP is used to convert human language into numbers that are understood by computer,Data Analysis is performed before processing data into machine learning models for accuracy and efficiency.We perform Data Analysis by performing data cleaning, preprocessing dataset in this project. 
Overview: Consumer Complaint Classification means classifying the nature of the complaint reported by the consumer. It is helpful for consumer care departments as they receive thousands of complaints daily, so classifying them helps identify complaints that need to be solved first to reduce the loss of the consumer. Here are the sequence of steps I followed in creating this project.

1. Data Analysis:
      1. We load dataset into dataframe using pandas.
      2. We identify unnamed columns and delete the unnamed columns(Axis =1).
      3. Now,we identify null values in the dataset. We delete entire row containing null values.
      4. We look for miss handling values in dataset. i.e, any values that are not related to columns.
2. Traning DataSet/Data Tokenization:
      1. We remove stopwords, stemmers, html tags, text in [], new lines, and text in other languages. This helps model in understaning words in efficient way. Based on the adjectives in sentence, it can change the meaning of sentence. And, to ignore case sensitive we convert all text into lower.
3.Splitting Data into train data and test data.
 1. We input the column names into machine learning model.
 2. We convert data from each column to numbers using Numpy.
 3. We count token words using CountVectorizer to identify the frequency of complaints.
 4. We split whole dataset into training data and test data. We train machine learning about feature and labels with trained data and test the accuracy on test data.
4. Machine Learning Model using  Stochastic Gradient Descent classification algorithm:
    1. we implement SGD classification on training data feature.
