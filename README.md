# Tengri News Clone 
Сайт можно посетить по ссылке  http://deqnqe.me/

## Введение
Этот проект направлен на репликацию ключевых функций сайта Tengri News, предоставляя упрощенную платформу для отображения новостных статей и  мультимедийного контента. Он разработан для демонстрации техник веб-разработки, включая веб-скрапинг, управление контентом и дизайн пользовательского интерфейса.

## Функции
- **Отображение Статей**: Демонстрирует новостные статьи с заголовками, содержанием, изображениями и датами публикации, также позволяет фильтровать по категориям “life”, “sport”, “auto”, “edu”, “travel”.
- **Функциональность Поиска**: Позволяет пользователям искать статьи по ключевым словам из заголовка и контента.

## Технологический Стек
- **Фронтенд**: HTML, CSS, JavaScript, Bootstrap
- **Бэкенд**: Flask (Python), MySQL
- **Веб-скрапинг**: BeautifulSoup, Selenium

## Настройка
Мой веб-сайт теперь успешно развернут и доступен для посещения по адресу http://deqnqe.me/.
Чтобы запустить этот проект локально, следуйте этим шагам:

1. **Клонировать Репозиторий**


2. **Установить Зависимости**
- Убедитесь, что на вашей машине установлен Python 3.8+.
- Установите необходимые пакеты Python:
  ```
  pip install -r requirements.txt
  ```

3. **Запуск Приложения Flask**
В файле app.py в функциях get_article_by_id(article_id), search_articles_in_db(query) и get_articles_from_db(tags) и в файле test5.py в функции save_articles_to_db(articles)поменять значения полей user, password, host, database, и создать схему news в MySQL чтобы подключиться к локальному MySQL. 
Запустить программу test5.py для парсинга сайта tengrinew.kz
Ввести в терминале команду 
```flask run```
Доступ к приложению по адресу `http://127.0.0.1:5000`.

## Использование
После запуска Flask приложения вы можете:
- Просматривать статьи на главной странице.
- Использовать строку поиска для поиска статей по ключевым словам.
- Фильтровать по категориям “life”, “sport”, “auto”, “edu”, “travel”

## Процесс проектирования и разработки
Сначала были собраны данные с оригинального сайта tengrinews.kz. Затем, воссоздала дизайн их веб-интерфейса, включая структуру заголовков, визуальное представление статей и цветовую схему сайта, обеспечивая тем самым узнаваемость и соответствие оригиналу. В процессе разработки добавляла функционал для поиска статей, фильтрации по категориям, времени, динамического парсинга. 

## Компромиссы
Чтобы ускорить процесс разработки я не парсила весь оригинальный сайт, но достаточно новостных статей, чтобы продемонстрировать функционал сайта. Также я не собрала комментарии, в будущем можно добавить функционал, чтобы отображать и добавлять комментарии. Также функция динамического парсинга замедляет процесс загрузки сайта. 


