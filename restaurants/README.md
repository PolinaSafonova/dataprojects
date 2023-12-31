# Проект: Рынок заведений общественного питания Москвы
**Цель проекта:** исследовать рынок питания Москвы и выявить особенности, которые помогут найти подходящее место для открытия нового заведения.  
Задачи:
- узнать, как распределяются заведения по категориям;
- выявить популярные сетевые заведения;
- проанализировать средние рейтинги и средние чеки заведений по районам;
- охарактеризовать кофейни и дать рекомендации для открытия нового заведения.

## Описание данных 
Датасет с заведениями общественного питания Москвы, составленный на основе данных сервисов Яндекс Карты и Яндекс Бизнес на лето 2022 года. Информация могла быть добавлена пользователями или найдена в общедоступных источниках.
Файл moscow_places.csv:
- name — название заведения;
- address — адрес заведения;
- category — категория заведения, например «кафе», «пиццерия» или «кофейня»;
- hours — информация о днях и часах работы;
- lat — широта географической точки, в которой находится заведение;
- lng — долгота географической точки, в которой находится заведение;
- rating — рейтинг заведения по оценкам пользователей в Яндекс Картах (высшая оценка — 5.0);
- price — категория цен в заведении, например «средние», «ниже среднего», «выше среднего» и так далее;
- avg_bill — строка, которая хранит среднюю стоимость заказа в виде диапазона, например:
«Средний счёт: 1000–1500 ₽»; «Цена чашки капучино: 130–220 ₽»; «Цена бокала пива: 400–600 ₽». и так далее;
- middle_avg_bill — число с оценкой среднего чека, которое указано только для значений из столбца avg_bill, начинающихся с подстроки «Средний счёт»
- middle_coffee_cup — число с оценкой одной чашки капучино, которое указано только для значений из столбца avg_bill, начинающихся с подстроки «Цена одной чашки капучино»:
- chain — число, выраженное 0 или 1, которое показывает, является ли заведение сетевым (для маленьких сетей могут встречаться ошибки): 0 — заведение не является сетевым, 1 — заведение является сетевым
- district — административный район, в котором находится заведение, например Центральный административный округ;
- seats — количество посадочных мест.

## Библиотеки и инструменты:
`Python` `Pandas` `Matplotlib` `Plotly` `Seaborn` `визуализация данных`

## Выводы:
- В Москве из заведений общественного питания преобладают кафе (всего 2376 штук) и рестораны (2042), на третьем месте оказались кофейни (1413). Менее всего популярны булочные (256) и столовые (315).
- Количество посадочных мест отличается в зависимости от категории: больше всего мест в ресторанах, барах/пабах, столовых и кафе. Меньше всего - в пиццериях и булочных.
- Сетевые заведения составляют 38,1% от всех объектов. В категориях "кофейня", "пиццерия" и "булочная" сетевых заведений больше, чем несетевых. Из топ-15 сетевых заведений семь являются кофейнями, два - пиццериями.
- Больше всего заведений находится в ЦАО, из них почти треть составляют рестораны. Почти во всех административных округах кафе на первом месте по количеству заведений, на втором - рестораны, на третьем - кофейни.
- Средние рейтинги заведений по категориям не сильно различаются: от 4,05 в категории "быстрое питание" до 4,39 в категории "бары/пабы".
- Самый высокий медианный чек составил 1000 р. в ЦАО и ЗАО, а самый низкий - 450 р. в ЮВАО.

## Рекомендации для открытия нового заведения
Наиболее удачный округ для открытия новой кофейни, судя по проведенному анализу, - это Западный. Всего в нем 150 заведений, причем 93 из них - сетевые. Покупателей может привлечь новое заведение с отличной от других концепцией. В Западном округе высокая средняя стоимость чашки капучино, а также высокий средний чек. Это позволит владельцам новой кофейни установить цены выше, чем в других районах (таких как, например, Юго-Восточный) и быстрее окупить затраты. Средняя стоимость чашки капучино в Западном округе составляет около 190 р., при открытии новой кофейни стоит ориентироваться на эту цифру. Можно понизить это число до 180, чтобы привлечь покупателей доступной ценой.
