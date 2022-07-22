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
## Supervised Machine Learning Model Prep
