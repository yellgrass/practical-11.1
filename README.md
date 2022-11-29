# practical-11.1

Link to notebook:
https://github.com/yellgrass/practical-11.1/blob/main/prompt_II.ipynb

Findings Summary:

After exploring the data somewhat, I dropped the features region, manufacturer, model and state as they had too many categories. I also changed the VINBool column to instead indicate the presence or absence of one, as the string itself did not appear too useful. After dropping outliers and plotting some graphs for visualization, I use a linear regression to model the data. 
From this linear regression and permutation importance, I found that year, odomter, type, cylinders and fuel appear to have the most influence on price and focused on those.
Running a ridge regression, which I determined to use an alpha of 6 for, on just these three features yielded a lower score, so I attempted to fit another linear regression model with those same features. 
The ridge model had a better fit than the second linear regression model.

Overall, I determined that the features year, odometer and type of car appear to have the most significant influence on price.
