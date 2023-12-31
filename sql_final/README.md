# **Проект: сервис для чтения книг**
**Цель:** проанализировать базу данных сервиса для чтения книг по подписке.

## Описание данных
Таблица books  
Содержит данные о книгах:
- book_id — идентификатор книги;
- author_id — идентификатор автора;
- title — название книги;
- num_pages — количество страниц;
- publication_date — дата публикации книги;
- publisher_id — идентификатор издателя.
  
Таблица authors  
Содержит данные об авторах:
- author_id — идентификатор автора;
- author — имя автора.

Таблица publishers  
Содержит данные об издательствах:
- publisher_id — идентификатор издательства;
- publisher — название издательства.

Таблица ratings  
Содержит данные о пользовательских оценках книг:
- rating_id — идентификатор оценки;
- book_id — идентификатор книги;
- username — имя пользователя, оставившего оценку;
- rating — оценка книги.

Таблица reviews  
Содержит данные о пользовательских обзорах на книги:
- review_id — идентификатор обзора;
- book_id — идентификатор книги;
- username — имя пользователя, написавшего обзор;
- text — текст обзора.

## Инструменты:
PostgeSQL

## Выводы: 
После 1 января 2000 года вышло 819 книг.  
Больше всего обзоров у книги "Сумерки" - 7 штук.  
Больше всего книг (42) выпустило издательство Penguin Books.  
Автор с самой высокой средней оценкой книг — Дж.К. Роулинг (средняя оценка: 4,4).  
В среднем пользователи, которые поставили больше 48 оценок, пишут 24 обзора.  
