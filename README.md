# Iris_Classification
A Iris Flower Classification  machine learning model using Logistic Regression, and python libraries like numpy, pandas, scikit-learn ,seaborn ,etc

Prerequisites:
1. Numpy- 1.19.3
2. Matplotlib- 3.3.2
3. Seaborn – 0.11.1
4. Pandas – 1.2.4
5. Scikit-learn – 0.24.2

STEPS:
1. Load the data
2. Analyze and visualize the dataset
3. Model training.
4. Model Evaluation.
5. Testing the model.


STEP 1: LOAD THE DATA
First, we’ve imported some necessary packages for the project.

Numpy will be used for any computational operations.
We’ll use Matplotlib and seaborn for data visualization.
Pandas help to load data from various sources like local storage, database, excel file, CSV file, etc.

Next, we load the data using pd.read_csv() and set the column name as per the iris data information.
Pd.read_csv reads CSV files. CSV stands for comma separated value.
df.head() only shows the first 5 rows from the data set table.

STEP 2: ANALYSE AND VISUALIZATION
To visualize the whole dataset we used the seaborn pair plot method. It plots the whole dataset’s information.
From this visualization, we can tell that iris-setosa is well separated from the other two flowers.
And iris virginica is the longest flower and iris setosa is the shortest.

Plotting the average feature of each class and separating the features from the target value.

Np.average calculates the average from an array.
Here we used two for loops inside a list. This is known as list comprehension.
List comprehension helps to reduce the number of lines of code.
The Y_Data is a 1D array, but we have 4 features for every 3 classes. So we reshaped Y_Data to a (4, 3) shaped array.
Then we change the axis of the reshaped matrix.
We used matplotlib to show the averages in a bar plot.
Here we can clearly see the verginica is the longest and setosa is the shortest flower.

STEP 3 : MODEL TRAINING
Using train_test_split we split the whole data into training and testing datasets. Later we’ll use the testing dataset to check the accuracy of the model.

Here we imported a support vector classifier from the scikit-learn support vector machine.
Then, we created an object and named it svn.
After that, we feed the training dataset into the algorithm by using the svn.fit() method.

STEP 4: MODEL EVALUATION
Now we predict the classes from the test dataset using our trained model.
Then we check the accuracy score of the predicted classes.
accuracy_score() takes true values and predicted values and returns the percentage of accuracy.

