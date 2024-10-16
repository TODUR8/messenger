### Новостной агрегатор для мобильных устройств.

Цель проекта построить базовую аналитику для мобильного приложения.

Стек технологий:
- Superset.
- PostgreSQL.
- Python(Pandas, numpy, scipy, hashlib, seaborn, matplotlib) 

Задачи:
- разработать базовый дашборд который покрывает основные аналитические запросы компании.
- Построить график Retention.
- С помощью А/B-теста оценить новый алгоритм рекомендации постов.
- Сформулировать выводы и рекомендации.

Результаты:

Описание данных:

Структура df_action
* user_id - id пользователя
* post_id - id поста
* action - действие пользователя
* time - время действия

Структура df_log
* user_id - id пользователя
* gender - пол
* age - возраст
* country - страна
* city - город
* os - операционная система
* source - источник пользователя
* exp_group - принадлежность к тестовой/эксперементальной группе


**Этап 1.** 
- Рассчитаем DAU, WAU и MAU. Вычислим средние значения этих метрик за весь период. Отобразим изменения метрик 
во времени на графиках.
Динамика общего числа пользователей
![Количество уникальных пользователей в день](https://github.com/TODUR8/messenger/blob/main/diagram/1_diagram.png)


![Количество уникальных пользователей в неделю](https://github.com/TODUR8/messenger/blob/main/diagram/2_diagram.png)


![DAU новые пользователи и старые пользователи](https://github.com/TODUR8/messenger/blob/main/diagram/3_diagram.png)


![Лайки и просмотры](https://github.com/TODUR8/messenger/blob/main/diagram/4_diagram.png)


![Средний CTR по дням](https://github.com/TODUR8/messenger/blob/main/diagram/5_diagram.png)


![Количество событий на одного пользователя](https://github.com/TODUR8/messenger/blob/main/diagram/6_diagram.png)



**Этап 2.** 
Построим график Retention.
Построим график новых, старых и ушедших пользователей по неделям.

![Retention по кагортам](https://github.com/TODUR8/messenger/blob/main/diagram/7_diagram.png)

На графики видим что в течение недели нам удается удержать примерно 20 процентов новых пользователей, а концу второй недели остается примерно 15 процентов. 


![График новых, старых и ушедших пользователей](https://github.com/TODUR8/messenger/blob/main/diagram/8_diagram.png)

**Этап 3.** 
С помощью А/B-теста оценим новый алгоритм рекомендации постов.

![пример](https://github.com/TODUR8/messenger/blob/main/diagram/1_diagram.png)

**Этап 4.** 
Сформулируем выводы.
