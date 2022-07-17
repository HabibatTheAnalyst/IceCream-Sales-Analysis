# Report

### Description
The project focused on IceCream sales. The dataset has two variables(temperature and revenue) and the aim was to determine statistically if temperature changes affects demands for IceCream and total revenue.

***
### Technology
* Google Sheet
* Jupyter Notebook
* Statistical measures

***
### Steps
Google Sheet was used to wrangle the dataset. The clean dataset was then uploaded to jupyter notebook for analysis. The data was loaded and statistical measures such as P-value and correlation were applied to derive at a the conclusion.

***
### Findings
- Analysing the summary of each column, the values of standard deviation for temperature and revenue are lower than their mean values. Therefore, further analysis will show more accurate estimates(i.e more reliable analysis).

```py
# Summary of each column
IceCream.describe()
```

<img src="https://user-images.githubusercontent.com/93320956/172587921-c43c6751-1b30-4298-9e5a-2b8437562668.png" width="300" height="300">

- Plotting temperature and revenue on line chart shows the linear correlation between the two variables i.e increase in temperature positively affects Icecream sales and ultimately revenue. This further births the question; does temperature often affects icecream sales in the given dataset or this is just a random occurence?

```py
# plot temperature against revenue
plt.scatter(data = IceCream, x = 'Temperature', y = 'Revenue', color = 'black', marker = 'v', alpha = 0.3)
plt.xlabel('Temperature', size = 16)
plt.ylabel('Revenue', size = 16)
plt.title('IceCream Sales', size = 16)
plt.yticks([0, 200, 400, 600, 800, 1000], ['$0', '$200', '$400', '$600', '$800', '$1000'], size = 13)
plt.xticks(size = 13)
plt.show()
```

<img src="https://user-images.githubusercontent.com/93320956/172589357-56c4b68c-6b46-4d82-bfce-065840e0ed16.png" width="300" height="300">

- On further analysis, I found out that the correlation values derived between temperature and revenue are closer to one. Hence, temperature and revenue are highly correlated with a correlation value of approximatelly 0.99. 

```py
# correlation between the two variables
IceCream.corr()
```

- Since correlation and causation are often mixed up because humans like to find patterns even when they do not exist, I took extra precautions to visualize the correlation. Because correlation charts that show causation can be effective.

```py
# temperaure and revenue correlation charts
sns.pairplot(IceCream)
```

<img src="https://user-images.githubusercontent.com/93320956/172591370-4f078f98-c146-426a-a897-59b407061c09.png" width="300" height="300">

- The correlation transformed into chart plots above better shows how linearly correlated the two variables are.

- To answer the question about randomness, I calculated the P-value which has a value equal to zero (0.0) which is less than 0.05.

```py
# p-value
from scipy import stats

r, p = stats.pearsonr(IceCream.Temperature, IceCream.Revenue)
print(round(r, 3))
print(p)
```

***
### Conclusion
Saying the p-value is 0% means our reults have a 0% chance of being attributed to random coincidence. Hence, from all the statistial results I could conclude that the data at hand supports my hypothesis. Therefore, there is a relationship between temperature and revenue and the increase in revenue is not due to randomness.