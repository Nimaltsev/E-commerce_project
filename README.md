# E-commerce_project
### Analysis of US online shop data

**Контекст и задача:**  
В данном проекте анализируются данные американского онлайн магазина, рассчитываются различные метрики и проводится RFM-анализ (в том числе Retention). 
Проект отвечает на вопросы
- Сколько пользователей, которые совершили покупку только один раз?
- Сколько заказов в месяц в среднем не доставляется по разным причинам? И выводится детализация по причинам
- По каждому товару определить, в какой день недели товар чаще всего покупается.
- Сколько у каждого из пользователей в среднем покупок в неделю (по месяцам)?
А также:
- Проводится когортный анализ
- Строится RFM-сегментация пользователей

**Используемый стек:**  
Python, pandas, seaborn, requests и другие

**Этапы работы:** <br> 
1. csv-файлы считаны с яндекс-диска и проведен EDA. В исходных данных 3 таблицы:
- df_custmrs - таблица с уникальными идентификаторами пользователей
- df_orders — таблица заказов, 
- df_items — товарные позиции, входящие в заказы
2. Проект последовательно отвечает на все вопросы, перечисленные выше, выводится визуализация ответов. Примем, что недоставленными считаются заказы, имеющие статусы "unavailable" и "canceled". Подробное описание каждого шага приводится в markdown-ячейках jupyter-ноутбука

**Результат:**  
Проведен анализ представленных данных (без использованя стат.методов), проведена RFM-сегментация и когортный анализ.
