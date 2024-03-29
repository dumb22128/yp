# Определение стоимости автомобилей

## Описание проекта
Сервис по продаже автомобилей с пробегом разрабатывает приложение для привлечения новых клиентов. В нём можно быстро узнать рыночную стоимость своего автомобиля. В вашем распоряжении исторические данные: технические характеристики, комплектации и цены автомобилей. Нам нужно построить модель для определения стоимости. 

**Заказчику важны:**
- качество предсказания;
- скорость предсказания;
- время обучения.

## Описание данных
**Признаки:**
* `DateCrawled` — дата скачивания анкеты из базы
* `VehicleType` — тип автомобильного кузова
* `RegistrationYear` — год регистрации автомобиля
* `Gearbox` — тип коробки передач
* `Power` — мощность (л. с.)
* `Model` — модель автомобиля
* `Kilometer` — пробег (км)
* `RegistrationMonth` — месяц регистрации автомобиля
* `FuelType` — тип топлива
* `Brand` — марка автомобиля
* `NotRepaired` — была машина в ремонте или нет
* `DateCreated` — дата создания анкеты
* `NumberOfPictures` — количество фотографий автомобиля
* `PostalCode` — почтовый индекс владельца анкеты (пользователя)
* `LastSeen` — дата последней активности пользователя

**Целевой признак:**
* `Price` — цена (евро)

## Задача
Необходимо построить модель для определения стоимости.
* Обучить разные модели. Для каждой попробовать различные гиперпараметры. (+ анализ скорости работы и качества моделей)
* Для оценки качества моделей применяем метрику `RMSE`.
* Значение метрики `RMSE` должно быть меньше `2500`.
* Изменять у модели только два-три параметра.
