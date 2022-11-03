### Уменьшение потребления электроэнергии  

Металлургический комбинат ООО «Так закаляем сталь» хочет уменьшить потребление электроэнергии на этапе обработки стали.  

**Цель проекта:**  
для этого он поставил задачу- определить наиболее важные признаки для определения конечной температуры стали на этапе её обработки.

**Описание проекта:**  
Для достижения цели были предприняты следующие основные шаги:  
1. Выгрузка данных и их превичный анализ.
2. Предобработка данных - выявление выбросов, аномалий и пропусков.  
3. Подготовка данных к обучению - масштабирование признаков и деление на выборки.
4. Обучение моделей, подбор параметров(случайный лес, линейная регрессия и дерево решений, градиентный бустинг)
5. Проверка на тестовой выборке, а также проверка на адекватность.

**Полученный итог:**  
Больше всего влияет на окончательную температуру стали: начальная температура, использованная энергия и время нагрева.  

**Использованные инструменты:**    
import numpy as np  
import pandas as pd  
import datetime  
import matplotlib.pyplot as plt  
from sklearn.ensemble import IsolationForest  
from sklearn.preprocessing import StandardScaler  
from sklearn.model_selection import train_test_split  
from sklearn.ensemble import RandomForestRegressor  
from sklearn.tree import DecisionTreeRegressor  
from sklearn.model_selection import cross_val_predict  
from sklearn.linear_model import LinearRegression  
from sklearn.dummy import DummyRegressor  
from sklearn.metrics import mean_absolute_error  
from sklearn.preprocessing import MinMaxScaler  
from sklearn.preprocessing import RobustScaler  
import lightgbm as lgbm  
from lightgbm import LGBMRegressor  
import time  
from sklearn.dummy import DummyRegressor  
