# Mushroom Project
## Selected Topic
The selected topic for our project is how to tell if a mushroom is poisonous or edible based on various features. And we want to determine which features should be used in the model 
## Reason for Topic
The reason we selected this topic is because there are 14,000 different species of mushrooms that come in different shapes, colors, textures, and sizes. It is important to be able to tell whether or not a mushroom is poisonous because certain poisonous mushrooms are dangerous when they are touched and there isn't any cure if a poisonous mushroom is consumed by accident. 
## Source for Data
The source of data we used for our project is a dataset that contains 22 columns and 8124 rows of different mushrooms and mushroom features. Theese columns consists of features of mushrooms that range from the color of the cap to the population or the habitat of the mushroom. According to the data set about 52% of the mushrooms are edible while 48% of them are poisonous. 
## Questions We Hope to Answer
The first question we want to answer is which supervised machine learning model is best for classifying edible or poisnous mushrooms. The second question we want to answer is if the features we keep are the most important ones and will they help give us the highest accuracy percentage possible. 
## Data Preprocessing and Feature Engineering
In order to the clean the data we from the CSV file and the Mushroom_df I made sure there were no NaN values in any of the rows or columns. The columns were all in lowercase so I changed all of them to uppercase so that it looks neater and changed the "class" column to "Edible or Poisonous". I did some research on which features are the most important when it comes to telling if mushroom is edible or poisonous.The features that were not important were dropped. One of the features that were important was the size,color,and surface of the cap while another feature was the size and color of the gill. These and the other important features were kept in the new dataframe. I then checked for any null values in the new dataframe and found there were NaN values in "Stalk-Root" column and those rows were dropped. Once those rows were dropped I verified that there were no more null values in the dataframe.
## Supervised Machine Learning Model 
The supervised machine learning model we decided to go with is the random forest model. This is because we are doing a binary classification(edible or poisonous) and we have more than 10 features for the model to sort through. One limitation of this model is that it is very complex because it creates by default 100 trees which uses up more resources and computing power. Some advantages of this model are there is no need for feature scaling and it can handle categorical values well. Before I trained the model I had to convert all of the string values because these models can only work with integers. To solve this I used the pd.get_dummies function and ended up creating more columns. This most likely affected the accuracy of the model. Then the data was split into train data and test data and in order to get a more accurate accuracy score I added a test_score parameter in the train_test_split function. The accuracy score ended up being 99.25% which was very high. I believe that in order to acheive a more realistic accuracy score is to use one-hot encoding to convert the string values to integers or using a model like the Distributed Random Forest.
## Results
We ran two different tests with the random forest model. The first test we used a dataframe that had no NaN which meant there were fewer columns that can be used in the train and test data. This was the result of the first test.

![image](https://user-images.githubusercontent.com/98357581/180584632-b0695c13-e301-455e-b18e-aa43fb702afb.png)

![image](https://user-images.githubusercontent.com/98357581/180584640-7376dc10-d26d-4207-86e7-93f13e94eb81.png)

The accuracy of our model ened up being 

The second test we ran was with the NaN values which meant we kept the original amount of columns from the original dataset. This was the result.

![image](https://user-images.githubusercontent.com/98357581/180584667-57f87fac-224f-4b31-9f6e-8e9e52193dbe.png)

![image](https://user-images.githubusercontent.com/98357581/180584675-43dc56d9-a831-4f6a-9524-4dffa289099e.png)

The first test has had a slightly better accuracy score than the second one. This is probably because of the NaN values that were used in the second test.
