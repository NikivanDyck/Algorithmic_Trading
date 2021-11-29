# Algorithmic Trading 
## Overview 
The use case of this project is to create an Algorithmic logic-based trading mechanism that defines when to buy or sell an asset and then execute that trading strategy. A logic-based trading mechanism is based on a set of conditions that, when triggered, initiate a buy or sell action.

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
Step 1: The training algorithm by adjusting the size of the training dataset.  Tuning the dataset was completed by updating the date offset value to one month, three months, six months.

Output: Changes in the short-long date of the trading window were better if the data offset was less than six months.  

Step 2: The trading algorithm was tuned by adjusting the simple moving average (SMA) that calculates the average price over a rolling period of a specific number of days.  

Output: SMA under 100 demonstrated better results vs. an SMA of 200 days.  

## Conclusion
A training set of three months, and a trading SMA of 4/100, had the overall best results. However, machine learning classifiers of Logistic Regression and Adaboot lowered the overall accuracy rating.  If a machine learning model is to be applied, additional research is required to find the best model. 

![ABplot](https://github.com/NikivanDyck/Algorithmic_Trading/blob/main/Plot_Images%20ab_plot.png)

## Addendum 

Resulting data plots

![1plot](https://github.com/NikivanDyck/Algorithmic_Trading/blob/main/Plot_Images%20ST_plot_1.png)  
![3plot](https://github.com/NikivanDyck/Algorithmic_Trading/blob/main/Plot_Images%20ST_plot_3.png) 
![3.1plot](https://github.com/NikivanDyck/Algorithmic_Trading/blob/main/Plot_Images%20ST_plot_3.1.png)
![6plot](https://github.com/NikivanDyck/Algorithmic_Trading/blob/main/Plot_Images%20ST_plot_6.png) 

