# TimeSeries-Taxi


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

# TimeSeries-Taxi


**Descrição do projeto

A empresa Sweet Lift Taxi coletou dados históricos sobre solicitações de táxi em aeroportos. Para atrair mais motoristas durante os horários de pico, precisamos prever a quantidade de solicitações de táxi para a próxima hora. 	
Crie um modelo para essa previsão.

_A métrica REQM no conjunto de teste não deve ser maior que 48.

## Descrição dos dados

Os dados são armazenados no arquivo `taxi.csv`. O número de pedidos está na coluna `num_orders`.

## Bibliotecas usadas
import **pandas** as pd

import **numpy** as np

import **matplotlib.pyplot** as plt

from **statsmodels.tsa.seasonal** import **seasonal_decompose**

from **sklearn.model_selection** import **train_test_split**

from **sklearn.metrics** import **mean_squared_error**

from **sklearn.linear_model** import **LinearRegression**

from **sklearn.model_selection** import **cross_val_score**

from **sklearn.model_selection** import **GridSearchCV**

## Conclusão final

**Análise
* O comportamento sazonal de todos os meses permanece estacionário.


* A linha de tendência sempre cresce com o passar dos meses, mas quando os meses mudam, há uma queda.


* Os dias da semana mais frequentes com a **menos** atividade de todos os meses são: **Terça-feira** em primeiro lugar em todos os meses e **Domingo** em segundo lugar em todos os meses, exceto abril.


* Os dias da semana mais frequentes com a **maior** atividade de todos os meses são: **Sexta-feira** em primeiro lugar em março, abril, junho, julho e agosto. **Segunda-feira** seguida em abril, maio, julho e agosto.

**Modelo
* O modelo de previsão de solicitações de táxi para a próxima hora teve um desempenho muito bom, com um RMSE de aproximadamente 8,43. Isso significa que nosso modelo tem uma margem de erro de 8,43 solicitações por hora, e nossa meta era inferior a 48, portanto, o desempenho foi excelente.
