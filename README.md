# HW_20_Supervised-Learing

Analysis

The purpose of this analysis was to determine if it was possible to distinguish healthy from high risk lows based on the available data and to what extent. Many factors were bought in to contribute to the prediction like total debt, number of accounts and borrower income. To see if we could make a dependable model to determine loan risk we started by splitting the loan status from the rest of our data leaving it as our target while the rest of the data was left as features. Then created a training and test group for the models. Using the training group to build the model was done in 2 ways. One was scaling all the data so different types of data did not have greater input based on the numeric value alone. The other left the data unscaled. After testing both models we found that scaling the data had a small increase in accuracy of .002%. I'm not sure this is significant and could be down to chance but it is an easy step to take.

-  Model 1 was un-scaled lbfgs model

-  Model 2 was scaled lbfgs

-  model 3 was scaled liblinear model

because there was no difference between model 3 and 2 i will just reference models 1 and 2

-  model 1 unscaled lbfgs
-  accuracy of 99.1% which is very high and I believe would suffice in these no life or death situations
-  had 100% precision identifying safe loans while identifying unsafe loans was only at 85%
-  The recall was slightly lower at 99% and 91%

-  Model 2 was scaled lbfgs
-  Scaling the data had a better result but only slightly with an accuracy of 99.3%
-  still had 100% precision determining safe loans while a slightly lower 84% finding unsafe ones
-  There was significant gains in recall in regards to unsafe loans though at 98%

Summary
I think scaling the data performed better based on its accuracy and significantly higher recall. It is most important to find dangerous borrowers as they will take a majority of resources to handle and the business needs to be ready when they default
