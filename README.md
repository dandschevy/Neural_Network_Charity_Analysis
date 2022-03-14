# Module 19 Challenge - Neural Network Charity Analysis
## Overview
The purpose of the Module 19 Challenge was to evaluate a data set of applicants and determine if a model can be created to predict if the candidates will be successful.  The following steps were taken for the analysis:
1.  Preprocess the data
2.  Compile, train, and then analyze the model
3.  Optimize

## Results
Based on the original data set, several columns were removed as they were not necessary.  These columns were EIN and name.  Once these were removed, the unique values were determined for the remaining columns.  The results were then binned and then separated into testing and training.  Once separated, the results were compiled and trained.  The results showed the model had a 72.4% accuracy rate.  The features selected for the model were application type, affiliation, classification, use case, organization, status, income amount, special considerations and ask amount.   
![image](https://user-images.githubusercontent.com/90434559/158096623-babafdd4-515e-49d4-9bad-fe8079d70c8e.png)

Since the results were lower than 75%, this provided an opportunity for optimization.  During the optimization process, three attempts were made to increase the model's accuracy to greater than 75%. Below is a summary of the three additional attempts:
1.  Optimizer 1 - This model removed only the name column and increased the epochs to 250.  This increased the accuracy to 73.4%.
![image](https://user-images.githubusercontent.com/90434559/158096989-479228f5-dd07-40b9-9001-840c5e003d23.png)

2.  Optimizer 2 - This model simply increased the epochs to 150.  However, with the additional epochs, the accuracy increased to 73.14%.
![image](https://user-images.githubusercontent.com/90434559/158097256-877de210-07ef-407b-a411-60e644eda86e.png)

3.  Optimizer 3 - The last model removed columns EIN, name, and affiliation with increased epochs to 150.  Unfortunately, this was the worst performing model with only 65.8% accuracy.  This is most like due to one of the features being removed.
![image](https://user-images.githubusercontent.com/90434559/158097451-25d530c9-b54e-471e-82de-467911cfdd83.png)

## Summary
In summary, the results could be optimized with additional epochs, but were still not as high as hoped.  With so many features, it may be beneficial to look into using a random forest model in order to determine if there are features that could be considered more predictive.
