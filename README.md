## **Project description**

Project to help steel plant to analisy and predict ladle temperature at the end of the production line to save costs on ladle heating to support metal smelting parameters

Project is made with **Python** and in **Jupyter Notebook** format.

<hr>

### **Main task**

In order to optimize production costs, some metallurgical plant  decided to reduce energy consumption at the steel processing stage.
You were asked to build a model that would predict the steel temperature of each ladle at the end of each batch. This would allow ladle overheating monitoring and prevent excessive heating to save energy.
We do have the following data to begin with:

### **Data description**

Data consists from files received from various sources:

* **data_arc_new.csv** — data about electrodes;
* **data_bulk_new.csv** — data about the supply of bulk materials (volume);
* **data_bulk_time_new.csv** — data about the supply of bulk materials (time);
* **data_gas_new.csv** — data on gas blowing through the alloy;
* **data_temp_new.csv** — data about temperature measurement;
* **data_wire_new.csv** — data about wire material (volume);
* **data_wire_time_new.csv** — data about wire material (time);

### **Реализация проекта:**
* Провела предварительный анализ (EDA) и предобработку данных. 
* Написала функцию для расчета Retention игроков.
* Использовала API для загрузки датасетов.
* Посчитала и проанализировала продуктовые метрики (Conversion Rate, ARPPU, ARPU).
* Проверила гипотезы, проанализировала результаты А/B-теста с использованием статистических тестов в Python(тест на независимость Хи-квадрат, T-test, Bootstrap).
* Визуализировала результаты в Python с применением seaborn и matplotlib.pyplot.
* Выбрала метрики для оценки результатов последнего прошедшего тематического события игры Plants & Gardens в компании, разрабатывающей мобильные игры.

<hr>

### **Замечание!**

Проект следует рассматривать как учебный. При работе с ARPPU и ARPU используется и T-test, и Bootstrap. Несомненно, в работе лучше выбрать что-то одно для однозначной трактовки результатов. 
