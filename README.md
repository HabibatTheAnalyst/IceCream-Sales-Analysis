# IceCream Sales Analysis

Anyone who is sugar tolerant wants the cold-sweet feel of ice cream. How it melts, flavor bursts in the mouth, and the cool feeling it gives during hot weather. Amidst this freshness, seasonality often has full control of how individuals demand or crave Ice cream.

### Hypothesis 
Increase in temperature affects IceCream sales

> ### The aim of this project was to determine statistically if temperature affects IceCream sales.

<img src="https://user-images.githubusercontent.com/93320956/171830868-18bee4f0-ee56-4a6e-8533-b49dbb2511c2.png" width="300" height="300">

---
### Table of Contents
* [Description](https://github.com/HabibatTheAnalyst/IceCream-Sales-Analysis/edit/main/README.md#description)
* [Technology](https://github.com/HabibatTheAnalyst/IceCream-Sales-Analysis/edit/main/README.md#technology)
* [Findings](https://github.com/HabibatTheAnalyst/IceCream-Sales-Analysis/edit/main/README.md#findings)
* [Conclusion](https://github.com/HabibatTheAnalyst/IceCream-Sales-Analysis/edit/main/README.md#conclusion)
* [Recommendation](https://github.com/HabibatTheAnalyst/IceCream-Sales-Analysis/edit/main/README.md#recommendation)

---
### Description
The project focused on IceCream sales. The dataset has two variables(temperature and revenue) with 500 rows. The aim was to determine statistically if temperature changes affects demands for IceCream as well as revenue.

---
### Technology
* GoogleSheet
* Python
* Statistical measures
#### steps
GoogleSheet was used to clean and wrangle the dataset. The clean dataset was then uploaded to jupyter notebook through command prompt. The data was loaded and statistical measures such as P-value and correlation were applied to derive at an hypothesis.

---
### Findings
- Analysing the summary of each column, the values of standard deviation for temperature and revenue are lower than their mean values. Therefore, further analysis will show more accurate estimates(i.e more reliable analysis).

<img src="https://user-images.githubusercontent.com/93320956/172587921-c43c6751-1b30-4298-9e5a-2b8437562668.png" width="300" height="300">

- Plotting temperature and revenue on line chart shows the linear correlation between the two variables i.e increase in temperature positively affects Icecream sales and ultimately revenue. This further births the question; does temperature often affects icecream sales in the given dataset or this is just a random occurence?

<img src="https://user-images.githubusercontent.com/93320956/172589357-56c4b68c-6b46-4d82-bfce-065840e0ed16.png" width="300" height="300">

- On further analysis, I found out that the correlation values derived between temperature and revenue are closer to one. Hence, temperature and revenue are highly correlated with a correlation value of approximatelly 0.99. 

- Since correlation and causation are often mixed up because humans like to find patterns even when they do not exist, I took extra precautions to visualize the correlation. Because correlation charts that show causation can be effective.

<img src="https://user-images.githubusercontent.com/93320956/172591370-4f078f98-c146-426a-a897-59b407061c09.png" width="300" height="300">

- The correlation transformed into chart plots above better shows how linearly correlated the two variables are.

- To answer the question about randomness, I calculated the P-value which has a value equal to zero (0.0) which is less than 0.05.

<img src="https://user-images.githubusercontent.com/93320956/172592983-ac8ff921-3dc9-4b07-9126-afc30d1a36b6.png" width="300" height="300">

---
### Conclusion
Saying the p-value is 0% means our reults have a 0% chance of being attributed to random coincidence. Hence, from all the statistial results I could conclude that the data at hand supports my hypothesis. Therefore, there is a relationship between temperature and revenue and the increase in revenue is not due to randomness. 

> ### I reject the null hypothesis thereby accepting the alternative hypothesis.

---
### Recommendation
stepss and tools used
the outcome 
conclusion and recommendation
link to the dataset
***link
Dataset - [here]()
