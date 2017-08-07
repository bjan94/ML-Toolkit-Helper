# Overview
**Statistical learning**: vast set of tools for understanding _data_.  
+ Supervised: Building a statistical model for predicting, or estimating an *output* based on one or more *inputs*. (Business, medicine, astrophysics, and public policy)
+ Unsupervised: There are inputs, but no supervising output. We can still learn relationships and structure from such data. 

[book website](http://www.statlearning.com)  

$$ Y = f(X) + \epsilon $$
***Why do we care about predicting $f$?*** 

1.**Prediction**: Usually inputs $X$ are readily available, but the output $Y$ cannot be easily obtained. $f$ is often treated as *black box* in the sense that one is not typically concerned with the exact $f$, provided it yields accurate $Y$.
  * **Example:** Suppose $X_1,...,X_p$ are charactersitics of a patient's blood samples. $Y$ is a variable encoding the patient's risk for a severe adverse reaction to a particular drug. The accuracy of $\hat{Y}$ as a prediction for $Y$ depends on two quantities : *reducible error*, and *irreducible error*. In general, the combination of the two errors fall to:
  $$E(Y-\hat{Y})^2 = E\[f(X) + \epsilon -\hat{f}(X)\]^2 \\
  				   = \[f(X) - \hat{f}(X)\]^2 + Var(\epsilon) $$
  which is essentially *reducible error* + *irreducible error*.

2. **Inference**: We are often interested in understanding the way $Y$ is affected as the independent variables change. We wish to estimate $f$, but not necessarily $Y$. Now, $\hat{f}$ cannot be a *black box* because we need to know the exact form of $f$. 
  * Consider a company that is interested in conducting a direct-marketing campaign. Goal is to identify individuals who will respond positively to a mailing. **Demographic variables** serve as predictors, and **response to the campaign** serves as the outcome. Company will be interested to know which media yields better results, how much increase in sales is associated with a given increase in advertising, etc.





