В данном проекте у "Бета-Банка" возникли проблеммы с оттоком клиентов, и маркетологи считают, что сохранить клиентов дешевле, чем привлечь новых.  
Из за этого возник этот проект, целю которого является создание модели, которая будет определять клиентов, которые могут уйти в ближайшее время.  
В ходе работы над данным проектом были предприняты следующие шаги:  
1. Загрузка данных и их первичный анализ.  
2. Исследование задачи(проверка баланса классов, масштабирование признаков и разбиение признаков на выборки).  
3. Обучение моделей с использованием различных методик борьбы с дисбалансов классов(увеличние и уменьшение выборки, взвешивание объектов и изменение порога классификации).
4. Тестирование модели и оценка значимости признаков.  

Результатом работы над данным проектом стала модель, обученная с помощью сбалансированных весов классов, а также с изменённым порогом классификации.

Использованные импорты:  
import pandas as pd  
import numpy as np  
from sklearn.preprocessing import StandardScaler  
from sklearn.model_selection import train_test_split  
from sklearn.metrics import mean_squared_error  
from sklearn.tree import DecisionTreeClassifier  
from sklearn.ensemble import RandomForestClassifier  
from sklearn.linear_model import LogisticRegression  
from sklearn.dummy import DummyClassifier  
from sklearn.metrics import f1_score  
from sklearn.utils import shuffle  
from sklearn.metrics import roc_auc_score  
from sklearn.metrics import roc_curve  
import matplotlib.pyplot as plt  
