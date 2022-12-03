## AB_testing

Here, we have been given a dataset that has information of users visiting a website and then subsequently whether they buy a product or not which is indicated by converted (1 - yes, 0 - No)  

Suppose our team came up with a new design of the website with the hope that more users would end up buing the product. As a Data Scientist, I would be curious to collect some data and make sure if we have data to support that claim. Hence we perform an A/B test. Fortunately, we have been provided the data set with 2 sets of groups - control (users shown old design) and treatment (users shown new design) groups. Each group should have unique set of users.   

Using AB testing, we determine if the claim is true. 

Test setup: 

Null hypothesis - The new version does not affec the conversion rate
Alternative hypothesis - The new design is different (or can say better) than the original website. 

Set alpha (significance value) = 0.5 , beta (Power) = 0.8. Lets say we want to see the improvements in conversion from 12% to 14%. This would be effect size.  

Based on the above values, the sample size can be determined (Refer plots to see how the this changes wrt alpha).  

After this, Z-test is performed to calculate the p-value. If p-value > 0.05, we fail to reject the null hypothesis. Otherwise we reject null hypothesis. 
