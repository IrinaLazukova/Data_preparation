# Исследование объявлений о продаже квартир

## Цель исследования:
Установить параметры, влияющие на ценообразование недвижимости в Санкт-Петербурге.

## Задачи исследования:

1. Получение данных. 
2. Предобработка, заполнение пропусков там, где это уместно.
3. Подсчет новых параметров и добавление их значения в таблицу:
    - цена квадратного метра;
    - день недели, месяц и год публикации объявления;
    - этаж квартиры (первый, последний, другой);
    - соотношение жилой и общей площади, а также отношение площади кухни к общей.
4. Исследование влияния на ценообразование следующих параметров: площади, числа комнат, удаленности от центра, даты размещения объявления. Построение гистограмм зависимости для каждого параметра.
5. Определение стоимости квадратного метра жилья в 10 населенных пунктах в окрестностях Санкт-Петербурга.
6. Определение границ центра Санкт-Петербурга и влияние этого фактора на цену недвижимости.
7. Выводы.

## Описание данных:
Данные сервиса Яндекс.Недвижимость — архив объявлений о продаже квартир в Санкт-Петербурге и соседних населённых пунктах за несколько лет.

- `total_images` — число фотографий квартиры в объявлении
- `last_price` — цена на момент снятия с публикации
- `total_area` — площадь квартиры в квадратных метрах (м²)
- `first_day_exposition` — дата публикации
- `rooms` — число комнат
- `ceiling_height` — высота потолков (м)
- `floors_total` — всего этажей в доме
- `living_area` — жилая площадь в квадратных метрах(м²)
- `floor` — этаж
- `is_apartment` — апартаменты (булев тип)
- `studio` — квартира-студия (булев тип)
- `open_plan` — свободная планировка (булев тип)
- `kitchen_area` — площадь кухни в квадратных метрах (м²)
- `balcony` — число балконов
- `locality_name` — название населённого пункта
- `airports_nearest` — расстояние до ближайшего аэропорта в метрах (м)
- `cityCenters_nearest` — расстояние до центра города (м)
- `parks_around3000` — число парков в радиусе 3 км
- `parks_nearest` — расстояние до ближайшего парка (м)
- `ponds_around3000` — число водоёмов в радиусе 3 км
- `ponds_nearest` — расстояние до ближайшего водоёма (м)
- `days_exposition` — сколько дней было размещено объявление (от публикации до снятия)

По каждой квартире на продажу доступны два вида данных. Первые вписаны пользователем, вторые — получены автоматически на основе картографических данных.

## Используемые библиотеки

pandas, numpy, matplotlib, seaborn
