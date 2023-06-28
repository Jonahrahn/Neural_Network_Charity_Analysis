# Neural_Network_Charity_Analysis

## Overview of Project:
he goal of this project was to clean, transform, and preprocess charity data for a Neural Network Model. After the ETL process, the model can be compiled, trained, and evaluated. With the initial model accuracy below 75 percent, optimization was necessary to improve the model's predictive capabilities.

## Resources
- AlphabetSoupCharity.ipynb
- AlphabetSoupCharity.h5
- AlphabetSoupCharity_Optimzation.ipynb
- AlphabetSoupCharity_Optimzation.h5
- charity_data.csv
----------------------------------------------------------------------
- Python(jupyter notebook)
- Pandas
- SciKit Learn
- Tensorflow
- Keras
- Pyspark


![image_name](images/layers_neurons.png)


## Results:


Data Preprocessing
Data Preprocessing: The targeted variable in the data was the "Is_successful" column. The features of the model included the following columns:

### Columns of Charity 
- ❌EIN-Identification number
- 📈NAME—Identification name
- ✅APPLICATION_TYPE—Alphabet Soup application type
- ✅AFFILIATION—Affiliated sector of industry
- ✅CLASSIFICATION—Government organization classification
- ✅USE_CASE—Use case for funding
- ✅ORGANIZATION—Organization type
- ✅STATUS—Active status
- ✅INCOME_AMT—Income classification
- ✅SPECIAL_CONSIDERATIONS—Special consideration for application
- ✅ASK_AMT—Funding amount requested
- Ⓜ️IS_SUCCESSFUL—Was the money used effectively

![image_name](images/accuracy.png)

The next step was compiling, training, and evaluating the model that lead to the accuracy above. This was originally due to the model not including the NAME column, and then modifying the neural net to increase the layers and neurons. In the end, the neural net included three hidden layers each in the order 440|40|10 because this increased the accuracy above the threshold of 75%. The activation functions used were Relu|Sigmoid|Sigmoid|Sigmoid. The model still had room for improvement in Data noise and Column Sorting even though it passed by 4%. 

Were you able to achieve the target model performance?
What steps did you take to try and increase model performance?

![image_name](images/accuracy_optimized.png)

## Summary:
hrough optimization efforts, the accuracy of the deep learning model was improved to 79%. The key optimization step was adding the sorted name data. Although increasing the number of layers and neurons had a minor impact on accuracy, further exploration and transformation of the data's noise and columns could potentially optimize the model even more. Sorting through the bins for rare occurrences in columns is recommended for better model performance. Overall, deeper data exploration and transformation have the potential to further increase accuracy.
