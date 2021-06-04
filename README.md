# Project3_mushrooms
My inspiration for this project was two fold: 1, a trip to Italy a few years ago where I saw locals foraging for mushrooms in the forest in Abruzzo and also finding strange mushrooms in my backyard or when out hiking. I have always asked myself, "I wonder if this mushroom is edible?" </br>
I used a mushroom csv dataset I found on kaggle to try create an app where the user could enter physical characteristics of their mushroom and the app would return an answer of edible (e) or poisonous (p). </br>
The dataset consisted of string character values which made things difficult to run decision trees.
Using get dummies we converted the X values which were all the characteristics into zeroes and ones (for present or not present and added extra columns).
I left the string values for the Y which was the class column edible or poisonous.
I train and tested the model and it came back with 100% accuracy.
The example code I found to use this type of format for the app used pickle as the database. 
I tried getting it to run only to realise that it came with an error for having string values present.
As I was running short on time and hot encoder didn't work, I manually updated the dataset to integer values.
I re-ran the model which was the same, and tried running the app but I had a syntax error "bash: syntax error near unexpected token `&' "
As I didn't want to have nothing to present, I plotted a few graphs in tableau with a few mushroom characteristics which were quite significant to determine if they were edible
or poisonous as this will be helpful for the targeted audience.
I had some troubles with push/pull requests with my github repo trying to merge files, so I created another repo which was successful.
I also wanted to try deploying what I had so far on Heroku.
