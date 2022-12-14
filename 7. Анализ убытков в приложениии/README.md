## Описание проекта
Несколько прошлых месяцев наш бизнес постоянно нес убытки. Нужно разобраться в причинах этой ситуации. В нашем распоряжении есть лог сервера с данными о посещениях приложения новыми пользователями, их покупки за этот период, а также статистика рекламных расходов. Необходимо изучить, как люди пользуются продуктом, когда они начинают покупать, сколько денег приносит каждый клиент, когда он окупается и какие факторы отрицательно влияют на привлечение пользователей.
Опишим возможные причины обнаруженных проблем и сформируем рекомендации для рекламного отдела. Рассматриваем данные от 1-го ноября 2019 года, в организации принято считать, что окупаемость должна наступать не позднее, чем через 2 недели после привлечения пользователей.

## Описание данных
**Таблица visits_log_short (лог сервера с информацией о посещениях сайта):**

- User Id — уникальный идентификатор пользователя
- Device — категория устройства пользователя
- Session start — дата и время начала сессии
- Session End — дата и время окончания сессии
- Channel — идентификатор рекламного источника, из которого пришел пользователь
- Region - страна пользователя

**Таблица orders_log_short (информация о заказах):**

- User Id — уникальный id пользователя, который сделал заказ
- Event Dt — дата и время покупки
- Revenue — выручка

**Таблица costs_short (информация о затратах на маркетинг):**

- Channel — идентификатор рекламного источника
- Dt — дата
- Costs — затраты на этот рекламный источник в этот день

## Используемые библиотеки
- pandas 
- numpy 
- matplotlib 