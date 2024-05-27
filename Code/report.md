# deep-learning-challenge

# Overview of the analysis:

    This data is comprised of more than 34,000 organizations who have received funding from fictional company Alphabet Soup. This model serves to use a binary classifier machine learning algorithm that can predict whether applicants will be successful if funded by Alphabet Soup.

# Results:

Data Preprocessing
    The feature variables for the model were:
        - APPLICATION_TYPE
        - AFFILIATION
        - CLASSIFICATION
        - USE_CASE
        - ORGANIZATION
        - STATUS
        - INCOME_AMT
        - SPECIAL_CONSIDERATIONS
        - ASK_AMT        
    The target variable for the model is:
        - IS_SUCCESSFUL
    The variables that were removed from the data:
        - EIN
        - NAME
        - STATUS
        - SPECIAL_CONSIDERATIONS

Compiling, Training, and Evaluating the Model
    Number of Neurons, Layers, and Activation Functions:
        - 3 Hidden Layers to capture the complexity of the dataset.
        - 171 Neurons( 80 in the 1st hidden layer, 60 in the 2nd hidden layer, 30 in the 3rd hidden layer, and one for the output layer)
            80 neurons were used in the first layer to better capture the high number of features and their interactions. The next two layers' number of neurons helped to reduce the features.
        - ReLU and Sigmoid Activation Functions
            ReLU is commonly used to help a machine learning model understand complex data and reduce the chances of gradients disappearing during back propagation. For our model, it works well to reduce the amount of data loss. The Sigmoid function is used in our binary classification to output the probability of an outcome between 0 and 1. 
    Target model performance:
        - This analysis was able to achieve target model performance before and after optimization methods. 
    Optimization steps:
        - In my attempts to optimize the ML model, I dropped columns from the original dataset that weren't necessary to determine success of the organization, I made the ASK_AMT column include more values into fewer bins to reduce variability in the features, and I added an extra hidden layer to the model with more neurons. 
    
# Summary: 

    Performance:
        The model before and after optimization achieved 100% accuracy. This means that the model learned the training data exceptionally well. The amount of loss was low before and after optimization as well. However, the amount of loss was lower in the optimized model the first time I ran both notebooks, but when I ran the first notebook again without additional changes, the loss was less in the pre-optimized model. 
    Recommendation:
        A Random Forest ML Model might be better for this model because it is more interpretable than Neural Networks and interpreting the data is the most important part of the model for data analysis. They can also show how certain featurs are more influential on the results. This could help our model by showing us which features can be manipulated to achieve greater accuracy and minimize loss.