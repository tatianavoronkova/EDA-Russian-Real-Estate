# EDA - Russia Real Estate 2018-2021

The dataset consists of lists of unique objects of popular portals for the sale of real estate in Russia. 
The dataset contains 540000 real estate objects in Russia.

## Features and data types:
> ### Categorical features:
> - **Region** (numerically encoded geographical area, identifies either a large city like Moscow or Saint Petersburg or a federal region / district)
> - **Building** type (numerically encoded type of building materials: 0 - Other, 1 - Panel, 2 - Monolithic, 3 - Brick, 4 - Blocky, 5 - Wooden)
> - **Object type** (apartment type: 1 - secondary real estate market, 11 - new building)
> ### Numerical features:
> - **Area** (total floor area of the apartment in sq. meters)
> - **Kitchen area** (kitchen area in sq. meters)
> - **Rooms** (number of rooms in the apartment, -1 stands for studios with open-space layout)
> - **Level** (floor the apartment is located on, could be treated as a categorical feature as well)
> - **Levels** (total number of storeys in the building)
> ### Geospatial features:
> - **Latitude** (geographical coordinate of the property)
> - **Longitude** (geographical coordinate of the property)
> ### Temporal features:
> - **Date** (date the listing was published)
> - **Time** (exact time the listing was published)

## Goal
Define the main factors and parameters influencing on apartments price in Moscow region based on data from service announcement for the period 2018-2021.

## Used Libraries
pandas, numpy, matplotlib, datetime

## Project Steps
1. Download and describe data
2. Clear and prepare data:
    - Find errors and outliers
    - Check duplicates and blanks
    - Add new columns
3. Data analysis:
    - Correlation matrix
    - Distribution chart for the main parameters
    - Dependance of ads on placement date
    - Dependance of price on placement date, rooms or level
  
## Conclusion
The selected dataset for Moscow region consist of **490,990 records**. The data is preprocessed in such a way as to eliminate outliers and save the most realistic records, covering **99% of real estate objects**.

**Main points:**

- An apartment price highly likely correlates with the total area, number of rooms and level in the building.
- The dynamics of offers in the real estate market are not stable. There is no seasonality trend in apartment sales from year to year. There is **decrease in offers** in the summer months **from May to August**.
- Since 2018 the average price per square meter has been continuously growing.
- The more rooms the lower price per square meter. This is true for the number of rooms from 1 to 6 inclusive.
- The dependence of price on the area can be divided into 2 conventional segments: up to 40 m2 and from 50 m2.
  - an apartment **up to 40 m2** inclusive costs above the regional average **92 thousand rubles** for square meter and usually presents studios and one-room apartments.
  - an apartment **from 50 m2** costs from **88 thousand rubles** for square meter and become more expensive as the total growth.
- As well the price directly depends on the floor of the apartment - **the higher floor, the more expensive the property**.

...
------


# Исследовательский анализ рынка недвижимости в России

Набор данных состоит из списка уникальных объявлений из популярного портала о продаже недвижимости в России. 
Набор данных содержит более 540,000 объектов недвижимости.

## Типы данных:
> ### Категориальные:
> - **Region** (числовой код, идентифицирующий либо крупный город, такой как Москва или Санкт-Петербург, либо федеральный округ)
> - **Building type** (числовой код, идентифицирующий строительный материал: 0 - Прочее, 1 - панель, 2 - монолит, 3 - кирпич, 4 - блоки, 5 - дерево)
> - **Object type** (тип недвижимости: 1 - вторичное жилье, 11 - новостройка)
> ### Количественные:
> - **Area** (общая площадь объекта в кв.м.)
> - **Kitchen area** (площадь кухни в кв.м.)
> - **Rooms** (количество комнат, “-1”обозначает квартиру-студию)
> - **Level** (этаж, на котором располагается квартира)
> - **Levels** (общее количество этажей в доме)
> ### Географические:
> - **Latitude** (широта)
> - **Longitude** (долгота)
> ### Временные:
> - **Date** (дата публикации объявления)
> - **Time** (время публикации)

## Задача:
Выявить основные параметры и факторы, влияющие на цену квартир в Московской области, используя данные объявлений из сервисов о продаже квартир за период с 2018 по 2021 год.

## Используемые библиотеки:
pandas, numpy, matplotlib, datetime

## Шаги:
1. Загрузка и описание данных
2. Очистка и подготовка данных:
    - поиск ошибок и выбросов
    - проверка дубликатов и пропусков
    - добавление столбцов
3. Анализ данных:
    - Корреляция данных
    - Распределение основных показателей
    - Зависимость объявлений от даты размещения
    - Зависимость цены от даты размещения, количества комнат, площади, этажа

## Заключение
По выбранному региону Московская область из всего датасета соответствовала выборка в **490,990 записей**. Данные предобработаны таким образом, чтобы исключить выбросы и оставить максимально реалистичные записи, покрывающие **99% объектов недвижимости**.

**Основные выводы:**

- Цена на объект больше всего коррелирует с общей площадью, количеством комнат и этажом размещения в здании.
- Динамика предложений на рынке недвижимости не стабильная. Не прослеживается тренд сезонности продложений о продаже квартир из года в год. Видно снижение предложений в летние месяцы **с мая по август.**
- С 2018 года средняя стоимость квадратного метра непрерывно растет.
- Чем больше комнат, тем ниже стоимость за квадратный метр. Это справедливо для количества комнат от 1 до 6 включительно.
- Зависимость цены от площади объекта можно разделить на 2 условных отрезка: до 40 м2 и от 50 м2.
  - объекты **до 40 м2** включительно стоят выше среднего значения по региону **92 тыс.руб** и включают в себя как правило студии и однокомнатные квартиры.
  - объекты **от 50 м2** уже стартуют **от 88 тыс.руб** и дорожают с ростом общей площади квартиры.
- Также цена прямо зависит от этажа размещения квартиры - **чем выше этаж, тем дороже объект**.

