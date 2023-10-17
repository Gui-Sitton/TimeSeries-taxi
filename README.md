# Taxi


**Project description**

The company Sweet Lift Taxi has collected historical data on cab requests at airports. To attract more drivers during peak hours, we need to predict the amount of cab requests for the next hour. 	
Build a model for this prediction.

_The REQM metric in the test set should not be higher than 48._

## Data description

The data is stored in the file `taxi.csv`. The number of orders is in the `num_orders` column.

## Libraries used
import **pandas** as pd

import **numpy** as np

import **matplotlib.pyplot** as plt

from **statsmodels.tsa.seasonal** import **seasonal_decompose**

from **sklearn.model_selection** import **train_test_split**

from **sklearn.metrics** import **mean_squared_error**

from **sklearn.linear_model** import **LinearRegression**

from **sklearn.model_selection** import **cross_val_score**

from **sklearn.model_selection** import **GridSearchCV**

## Final Conclusion

**Analysis**
* The seasonal behavior of all the months remains stationary.


* The trend line always grows as the months go by, but when the months change there is a drop.


* The most frequent days of the week with the **least** activity of all the months are: **Tuesday** in first place in all months and **Sunday** in second place in all but April.


* The most frequent days of the week with the **most** activity out of all the months are: **Friday** in first place in March, April, June, July and August. **Monday** followed in April, May, July and August.

**Model**
* The model for predicting taxi requests for the next hour performed very well, with an RMSE of approximately 8.43. This means that our model has a margin of error of 8.43 requests per hour, and our target was less than 48, so performance was excellent.
