# deep-learning-challenge

This ReadMe serves to:
   1. Certify that this work is my own,
   2. Specify code source and its location in my 'deep-learning-challenge' repository,
   3. Explain the process of the challenge

1. 
My name is Brittney Watts, and I am in the UNCC/EdX Data Analytics Bootcamp. This challenge is a product my own work.

2. 
The source code is my interpretation of the information we have learned in class with some help from class activities, and here
is a breakdown of the locations of each element of my assignment:

    deep-learning-challenge
        .ipynb_checkpoints
        CODE
            .ipynb_checkpoints
            AlphabetSoupCharity.ipynb
            AlphabetSoupCharity_Optimization.ipynb
            report.md  
        Output
            AlphabetSoupCharity.h5
            AlphabetSoupCharity_Optimization.h5
        .gitignore
        README.md

Home_Sales:
   My task was to read the data from the "charity_data.csv" file and use Scikit-learn to preprocess the data and compile, train and evaluate the machine learning model to predict whether applicants will be successful if funded by Alphabet Soup.
   
3.
Steps:     

    - Read in the charity_data.csv into a Pandas DataFrame
        - Identify the features and target variables for the model
    - Drop the EIN and NAME columns
    - Find out the unique values for each column and combine "rare" categorical variables together in the columns where there are too many unique datapoints.
    - Encode categorical variables
    - Split the data into a features array(X) and a targey array (y). Then use train_test_split to split the data into training and testing data. 
    - Scale the training and testing features with a StandardScaler() instance, fit, and transform.

    - Create a Neural Network model with hidden layers and activation functions.
    - Create an output layer
    - Check the structure of the model.
    - Compile and train the model.
    - Be sure to create a callback function that saves the model's weights every five epochs.
    - Evalueate the model to determine accuracy and loss.
    - Export the results tot an HDF5 file.

    - Optimize the model
