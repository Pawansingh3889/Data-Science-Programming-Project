Module Name: Data Science Programming

Task:

Olympic Games (50%)
For this task you will need to download the csv file ‘Olympic Games.csv’ from Blackboard. The file ‘Olympic Games.csv’ contains the medals won by athletes at the Olympic games between 1920 and 2016. The file ‘Olympic Games.csv’ has 15 columns: ID, Name, Sex, Age, Height, Weight, Team, NOC, Games, Year, Season, City, Sport, Event and Medal.
For this task you need to write a code to do the following:
(a) Read in the csv file ‘Olympic Games.csv’ to create a dataframe. Remove the columns named ‘ID’,‘Name’,‘Team’,‘Games’ and ‘City’. Further, remove all the rows which have ‘NA’ in the ‘Medal’ column. In the ‘Sex’ column, convert all of the ‘M’s to 0 and all of the ‘F’s to 1. In the ‘Season’ column, convert all of the ‘Summer’s to 0 and all of the ’Winter’s to 1. In the ’Medal’ column, convert all of the ‘Gold’s to 3, all of the ‘Silver’s to 2, all of the ‘Bronze’s to 1. After World War II Germany was split into the East and West so in the ‘NOC’ column, convert all of the ‘FRG’s to ‘GER’ and convert all of the ’GDR’s to ’GER’. In the 1990’s USSR split into several countries. As Russia has invaded Ukraine please remove all the rows which have ‘NOC’ equals ‘URS’ or ‘RUS’.
(4 marks)
(b) Remove all ‘NOC’ which appear less than 25 times. Using Matplotlib:
(i) Create a histogram of the frequency of countries against number of medals using 10 bins.
(ii) Create a histogram of the frequency of countries against number of gold medals using 10 bins.
(iii) Create a histogram of the frequency of countries against number of points using 10 bins, where points equals the sum of the number of bronze medals plus twice the number of silver medals plus three times the number of gold medals.
 Comment on these results. (c) Using Matplotlib:
(i) Create a bar chart of the number of medals for each sex. (ii) Create a bar chart of the number of medals for each season.
(iii) Create a histogram of the frequency of the athletes age. (iv) Create a histogram of the frequency of the athletes height. (v) Create a histogram of the frequency of the athletes weight.
(6 marks)
Comment on these results.
(6 marks)
2
(d) Remove all the rows which have ‘NaN’ in the ‘Height’ or ‘Weight’ columns. Make a scatter plot of ‘Weight” and ‘Height’ and colour the points using ‘Sex”. Create a new column called ‘BMI’ equal to the ‘Weight’ divided by the (‘Height”/100)2. Make a scatter plot of ‘BMI’ and ‘Weight’ and colour the points using ‘Sex’. Create a correlation matrix and discuss your results.
(6 marks)
(e) When ‘Sex’ equals 0, remove all rows with ‘Age’ greater than 43, or ‘Age’ less than 18, or ‘Height’ less than 158, or ‘Height’ greater than 205, or ‘Weight’ less than 52 or ‘Weight’ greater than 120. When ‘Sex’ equals 1, remove all rows with ‘Age’ greater than 39, or ‘Age’ less than 15, or ”Height” less than 148, or ‘Height’ greater than 193, or ‘Weight’ less than 40 or ”Weight” greater than 94. Remove rows with ‘Year’s less than 1948 and remove ‘Season’s equal to 1. Remove the ‘Season’ column. Now remove ‘Sports’ which have less than 200 medals. Using Matplotlib make a bar chart of the number of medals in each ‘Sport’. Comment on this. Now remove the ‘Events’ column. Name your dataframe ‘dfe’. (6 marks)
(f) Normalise the ‘Age’, ‘Height’, ‘Weight’, ‘Year’, ‘Medal’ and ‘BMI’ columns. In this part of the question just consider the case when the ‘Sport’ equals ‘Baseball’. You should split the data into (80%) training data and (20%) test data. Use an appropriate linear model from sklearn to predict ‘NOC’ using the normalised values ‘Sex’, ‘Age’, ‘Height’, ‘Weight’, ‘Year’, ‘Medal’ and ‘BMI’. Test your model using the test data set. Comment on your results.
(6 marks)
(g) You are now going to try to predict ‘NOC’ when the ‘Sport’ column is ‘Base- ball’. Now split the data into (80%) training data and (20%) test data. Create any regression model you like using PyTorch, select an appropriate criterion, optimisation algorithm, and learning rate. Train the model and report the training error. Comment on the testing error. (6 marks)
(h) Using your dataset obtained in Q1(e), create a new dataframe called ‘new df’. Create a list called ‘Rownames’ using the 69 ‘NOC’ values which you will use as the row names. Create a list called ‘Columnames’ using the 22 ‘Sport’ values which you will use as the column names. The values in ‘new df’ should represent the total number of points (i.e. the total of the ‘Medal’ number) each ‘NOC’ gets in each ‘Sport’. Obtain the correlation matrix of ‘new df’. Discuss your results. Write ‘new df’ to a csv file and read this into R. In R, create 4 different plots to illustrate some statistical properties of ‘new df’. Discuss any
significant results.
