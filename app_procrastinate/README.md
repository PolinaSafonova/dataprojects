# Проект: Анализ бизнес-показателей
**Цель проекта:** узнать причины убытков рекламы в приложении Procrastinate Pro+.  
Задачи: 
- составить портрет пользователей;
- посмотреть расходы на маркетинг по различным рекламным каналам;
- определить, какие каналы окупаются и не окупаются.

## Описание данных
Файл visits_info_short.csv хранит лог сервера с информацией о посещениях сайта.
- User Id — уникальный идентификатор пользователя,
- Region — страна пользователя,
- Device — тип устройства пользователя,
- Channel — идентификатор источника перехода,
- Session Start — дата и время начала сессии,
- Session End — дата и время окончания сессии.

Файл orders_info_short.csv хранит информацию о заказах.
- User Id — уникальный идентификатор пользователя,
- Event Dt — дата и время покупки,
- Revenue — сумма заказа.

Файл costs_info_short.csv хранит информацию о расходах на рекламу.
- dt — дата проведения рекламной кампании,
- Channel — идентификатор рекламного источника,
- costs — расходы на эту кампанию.

## Библиотеки и инструменты:
`Python` `Pandas` `Matplotlib` `NumPy` `когортный анализ` `юнит-экономика` `продуктовые метрики`

## Выводы:
Мы проанализировали рекламу в приложении Procrastinate Pro+. Для этого мы узнали, в каких странах находятся пользователи приложения, какими устройствами пользуются, какими каналами они были привлечены. Основная доля пользователей - из США, которые предпочитают использовать мобильные устройства. Платящих клиентов больше среди юзеров Mac и iPhone. В большинстве случаев они привлекаются органически, а также через каналы Faceboom и TipTop.
Далее мы узнали, что, несмотря на солидные вложения, реклама не окупается, и проверили, по каким причинам. Во-первых, бюджет был потрачен впустую на TipTop и Faceboom - при высокой стоимости привлечения клиента они совсем не окупаются. Во-вторых, в Европе низкая конверсия пользователей.
Рекламному отделу стоит пересмотреть каналы привлечения: отказаться от AdNonSense, направить бюджет в RocketSuperAds, YRabbit, MediaTornado. Стоит снизить значительно снизить траты на Faceboom и TipTop и придумать новую рекламу: вряд ли стоит отказываться от них совсем, так как они приводят много пользователей. Также нужно продумать стратегию, как конвертировать органических пользователей: они составляют большую часть клиентов приложения, не требуют затрат на привлечение, а значит, потенциально могут принести хорошую прибыль.
