# Project3_mushrooms
My inspiration for this project was two fold: 1, a trip to Italy a few years ago where I saw locals foraging for mushrooms in the forest in Abruzzo and also finding strange mushrooms in my backyard or when out hiking and finding myself asking "I wonder if this mushroom is edible?".  

I used a mushroom csv dataset I found on kaggle to try create an app where the user could enter physical characteristics of the mushroom they had found and the app would return an answer of edible (e) or poisonous (p). I thought people who went shrooming as a hobby would find this app useful.  

The dataset consisted of categorical data (string character values) which made things difficult to run decision trees. Using get dummies I converted the X values which were all the characteristics of the mushrooms into zeroes and ones (for present or not present which added extra columns). I left the string values for the Y which was the class column edible or poisonous. I trained and tested the model and it came back with 100% accuracy. I also tested the data to see if any features were more significant than others, but they were all of a similar weighting.  

The example code I found to create the app which was I thought was suitable for this type of dataset used pickle as the database. I tried getting it to run only to realise that it came back with an error for having string values present. As I was running short on time and hot encoder didn't work either, I manually updated the dataset to integer values in excel using the find and replace feature. I re-ran the model which gave the same result, and tried running the app but I had a syntax error "bash: syntax error near unexpected token `&' "  

As I was running short on time, I parked troubleshooting the app further as I didn't want to have nothing to present for my project. I plotted a few graphs in tableau with a few mushroom characteristics which had some noteable outcomes to determine if they were edible or poisonous as I thought this will be helpful for the targeted audience in the meantime.  

I had some troubles with push/pull requests with my original github repo trying to merge files, so I created another repo which was successful. https://github.com/Andie009/Project3_mushrooms  

I tried to deploy the html files I had made even if the model page was not working correctly on Heroku through the url https://mushroominformation.herokuapp.com/  
The app passed the build, release and deploy stages, however unfortunately when I went to view it, it came up with an application error.  

If I had more time I would work on the following things to improve this project:  
Use CSS styling to beautify the website, I would create more user friendly inputs such as a colour wheel or cap shape images to select from on the model webpage, improve the formatting on the charts so users don’t have to refer to the legend down the bottom, I would try using another database such as SQLite to see if that would get the app working and troubleshoot the application error on Heroku.
