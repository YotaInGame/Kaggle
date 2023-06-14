# Прогнозирование болезни сердца

Одна из основных задач в этом наборе данных - предсказать на основе заданных характеристик пациента, есть ли у этого конкретного человека заболевание сердца или нет, а другая - экспериментальная задача по диагностике и получению различных сведений из этого набора данных, которые могли бы помочь в большем понимании проблемы.

Перед построением моделей выбрали метрику Recall, т.к важнее определить больше больных или возможно больных пациентов

*Данный проект был выполнены в ходе обучения на программе "Специалист по Data Science plus" в Мастерской Практикума.*

| Описание           | Используемые библиотеки                     |
| :--------------------- |:---------------------------|
| Это многомерный тип набора данных, который означает предоставление или вовлечение множества отдельных математических или статистических переменных, многомерный числовой анализ данных. База данных Кливленда на сегодняшний день является единственной, используемой исследователями ML. | pandas, numpy, pandas_profiling, Image, matplotlib, plotly, sklearn, RandomForestClassifier

## Вывод

В ходе проделанной работы были выполнены следующие шаги.
- Был составлен план проекта и его цели.
- Заполнены пропуски, убраны выбросы.
- Проведен исследовательский анализ данных
- Построены базовые модели
- В каждом этапе присутствует визуализация данных.
- Выбрана лучшая модель на основе базовых, добавлена кросс валидация и балансировка классов.

Были обучены три базовые модели Logreg, Des. Tree, Random Forest:
| Модель           | Recall|
| :--------------------- |:---------------------------|
|Решающее дерево|0.821053|
|Лог. регрессия|0.831579|
|Случайный лес|	0.905263|

Выбрана лучшая базовая модель **Случайного леса** и улучшена балансировкой классов и Кросс валидацией, в результате получена след.метрика:

* Recall **0.915789**.


