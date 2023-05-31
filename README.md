# Хакатон: Битва Titанов,  кейс: Система прогнозирования отказов и инцидентов на объектах железнодорожной инфраструктуры, заказчик: РЖД
# Стек технологий
1. Python
2. UMAPP
3. CatBoost
# Решение
1. После анализа датасета, мы выявили в нем очень большое количество признаков, не имеющих корреляцию между собой и целевой переменной.<br>
2. Мы решили снизить размерность датасета с помощь технологии UMAPP, он отображает данные на n-размерном измерении. После правильного отображение можно заметить отчетливое разделение признаков<br>
![umapp](https://github.com/IsMarshev/Case-RZD-Battle-of-Titans/blob/main/src/umapp.png)
3. Дальше мы приступили к обучению модели, и предсказанию. Для обучения мы взяли два классификатора Catboost и SVC. В итоге Catboost дал нам больше точности, f1-score(macro) = 0.9849
![score](https://github.com/IsMarshev/Case-RZD-Battle-of-Titans/blob/main/src/image.png)
График предсказаний и реальных отказов
![pred](https://github.com/IsMarshev/Case-RZD-Battle-of-Titans/blob/main/src/%D0%B8%D1%82%D0%BE%D0%B3.jpg)
4. Создание рекомендательной системы
![rks](https://github.com/IsMarshev/Case-RZD-Battle-of-Titans/assets/114869741/e887f2dc-b8f4-43d5-8c54-9e8b98f3f177)
