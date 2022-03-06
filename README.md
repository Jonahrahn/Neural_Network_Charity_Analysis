# Neural_Network_Charity_Analysis

## Overview of Project:
The goal of this project was to clean, transform, and preprocess charity data for a Neural Network Model. After the ETL process, the model can be compiled, trained, and evaluated. After running the first model, there was a need to increase the model accuracy above 75 percent to optimize the model to more accurtely predict.

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
The data contained many columns to sort through but after exploration, the "Is_succcesful" was the targeted variable. The features of the model were the column names below in green. The NAME column was retroactively restored to increase the models prediction accuracy. The EIN was in the end removed because it was not expected to add any bit of information to the dataset.

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

The next step was compiling, training, and evaluating the model that lead to the accuracy above. This was originally due to the model not including the NAME column, and then modifying the neural net to increase the layers and neurons. In the end, the neural net included three hidden layers each in the order 440|40|10 , because this increased the accuracy above the threshold of 75%. The activation functions used were Relu|Sigmoid|Sigmoid|Sigmoid. The model still had room for improvement in Data noise and Column Sorting even though it passed by 4%. 

Were you able to achieve the target model performance?
What steps did you take to try and increase model performance?

![image_name](images/accuracy_optimized.png)

## Summary:
The results of the deep learning model showed that the due to the optimization, we were able to ge the accuracy to 79%. The key bit off optimization was adding the sorted name data, while adding extra layers and neurons only increased the accuracy by a fraction. Some reccomendations that I would provide for people attempting to optimize the model even more would be sort through the bins for rare occurrences in columns. The difference in creating a better model could have also been solved with a deeper exploration of the data and the noise and columns could have been transformed to optimize for higher accuracy.
