# bolid.team
 
# Дашборд по продажам для компании “Bolid.Team”


Группа компаний Bolid Team работает на рынке аттракционов и развлечений с 2002 года. Деятельность компании включает 3 направления: 

- производство аттракционов, 
- эксплуатация аттракционов,
- производство мягких призовых игрушек.



## Задача

Требуется создать дашборд в DataLens, который позволит анализировать продажи услуг аркадных аттракционов - как верхнеуровнево, так и в разрезе объектов и аттракционов.

На данный момент дашборд будет строиться на исторических данных, в дальнейшем планируется подключение к базе данных и обновление информации в режиме реального времени.

Для построения дашборда используется выгрузка информации о чеках и товарных позициях с сайта https://platformaofd.ru/ за 2022 г и январь - август 2023 гг.

Требуется построить дашборд в Yandex.DataLens.

**Основные пользователи** - руководители компании. Дашборд будет использоваться для определения прибыльных аттракционов, групп аттракционов и объектов, а также определения сезонных трендов.

### Основные метрики для построения дашборда

- общая выручка (индикатор);
- общее количество проданных услуг (индикатор); 
- общее количество чеков (индикатор);
- среднее количество позиций в чеке (индикатор);
- средняя цена проданной услуги (метрика используется вместо метрики среднего чека)  (индикатор);
- доля по группам цен (для просмотра, какая доля услуг продается по минимальной цене) (кольцевая диаграмма);
- выручка по способу расчета (доля наличных и электронных платежей) (кольцевая диаграмма);
- выручка по признаку расчета (доля приходов и возвратов)  (кольцевая диаграмма).


### Дополнительные метрики

**Изменение метрик в динамике:**
- выручка (расчет скользящего среднего для прогноза трендов; сравнение выручки с предыдущим периодом) (линейная диаграмма);
- количество проданных услуг, чеков и средняя цена услуги (линейная диаграмма);
- доля по группам цен (нормированная диаграмма).
Метрики средних продаж по часам, дням, неделям, месяцам, годам:
- средняя выручка (индикатор);
- среднее количество проданных услуг (индикатор);
- среднее количество чеков (индикатор);
- средние продажи на объект (индикатор);
- средние продажи на аттракцион (индикатор);
- средние продажи в час, в день недели, в месяц, в квартал, в год (линейная диаграмма).

Показать на графиках отклонение от среднего в абсолютах и в процентах.

Можно добавить на дашборд дополнительные графики (таблицы, иерархии), которые помогут провести анализ продаж

### Уровень детализации

**Ключевые показатели**  - города - объекты - группы аттракционов - аттракционы

**Фильтры и срезы данных**

Фильтры:

- Дата;
- Город;
- Объект;
- Группа аттракционов;
- Аттракцион

Срезы:

- Дата (по часам, дням, неделям, месяцам, годам);
- Город;
- Объект;
- Группа аттракционов;
- Аттракцион.



## Описание данных

**Файл items.csv**

Файл содержит информацию о товарных позициях в чеках за период с 1 января 2022 г. по 21 августа 2023 г.

**Файл checks.csv**

Файл содержит информацию о кассовых чеках за период с 1 января 2022 г. по 21 августа 2023 г.


## Инструменты
*DataLens*

## Ссылка на дашборд

https://datalens.yandex/cghjmnzx0u4i1 