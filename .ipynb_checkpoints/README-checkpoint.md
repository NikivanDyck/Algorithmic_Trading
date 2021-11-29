# Algorithmic Trading 
## Overview 
The use case of this project is to create an Algorithmic logice based trading trading mechinisum that defines when to buy or sell an asset and then execute that trading strategy. This means that it’s based on a set of conditions that, when triggered, initiate a buy or sell action.


## Data
The following models were reviewed 

|Training set size | Short/Long | SMA Accuracy (f1 score) | ML Classifier Used |  ML Accuracy |  Actual vs Stratagy % | 
| :---: | :---: | :---:  | :--- | :--: | :--:|
|1 month | 4/20 | 56% | Logisic Regression| 52% | -4 |
|3 months | 4/20 | 54% | AdaBoost| 52% | -2 |
|3 months | 4/100 | 55% | Logistic Regression| 52% | -3 |
|3 months | 4/100 | 55% | AdaBoost| 55% | 0 |
|3 months | 4/200 | 47% | Logistic Regression | 52% | 5 |
|6 months | 4/100 | 56% | AdaBoost| 53% | -2 |
|6 months | 4/200 | 53% | Logistic Regression | 48% | -5 |
|6 months | 4/200 | 53% | AdaBoost| 52% | -1 |

## Steps followed to review data
Step 1: Tune the training algorithm by adjusting the size of the training dataset.  This was completed by adjusting the size of the training dataset, This was completed by updating the date offset value to 1 month, 3 months, 6 months

Output: Changes in the short long date of the trading window were better if they we set less than 6 months.  

Step 2: The trading algorithm was tuned by adjusting the simple moving average (SMA) that calculates the average price of a stock over a rolling period of a specific number of days.  The following averages were used. 

Output: SMA under 100 has better results.  

## Conclusion
The data reflects that and taining set of 3 months, SMA of 4/100 had the over all best results.  Maschaile claering classificers if Logistic Regression and Adaboot lowered the overall accuracy rating. 

[Plot_Images ab_plot.png]

## Addendum 

Resulting data plots

[Plot_Images ST_plot_1.png], [Plot_Images ST_plot_3.png],

[Plot_Images ST_plot_3.1.png],[Plot_Images ST_plot_6.png] 

