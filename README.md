# Beer Data analysis
 This project throws emphasis on dealing with beer data  and finding out  the factors that contribute to beer overall rating . It takes in consideration various factors and transforms the reviews written down with the form of sentiments with the help of sentiment analysis . After doing this linear regression is performed onto the data set . 
 The error recorded is 0.3
 
# cleaning the data 
Date is transformed into datetime as the date is received in seconds 
Year is extracted from the  datetime in order to work towards EDA
Null abv values are replaced by mean alchol to beer value as this  value cannot be null
Null reviews and strings are replaced by no values

# EDA to extract inisghts from data 

39.184k beers have beer_ABV ranging from **4.98-5.02**. The data is positively skewed . This value is similar when null values are replaced with mean as this is important in determining how strong a beer is value

*Schorschbräu Schorschbock 57% * on an average has  the highest ABV

Again brewer with brewerid 6513 is on top with producing strongest beer Schorschbräu Schorschbock 57% of beer style Eisbock with beer ABV content of 57.7%.

Followed by brewerid:35 for** Samuel Adams Utopias** of style American Strong Ale

Followed by 16866

Year 2000 enjoyed the highest overall rating on an average.

with the help of  corrplot , We can conclude that following is the order of important ratings among taste,aroma, appearance, and palette that helps determine overall rating.

Aroma.
Taste.
Palette.
Appearance.



# prediction model creation
Sentiment analysis helps us determine Samuel Adams Scotch Ale,Maudite,Abita Select Four Grain are the good beers based on the sentiment of the  reviews 
It is  also required so that reviews can be used as a numeric factor to determine the overall rating 
train  test and validation sets are use to avoid  bias during model training ad hyperparamter tuning
datetime is converted 
beer style is column that cant be dropped as style influences appearences and overall  review so hence it is convrrted using one hot encoding 

Linear regression is implemented and validation set is find out how accurate the  model is  and hyperparameter tuning is done to improve performance

# Conclusion:
It was found out that certain beer  styles along with  aroma , Taste , Palette and Appreance were the important factors, apart from that the error recorded was only  0.3 meaning the model was 70 % accurate 
