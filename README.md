# Лабораторная работа № 2 "Анализ и проектирование" по дисциплине "Основы разработки Web-приложений"

***"Кинопоиск-мини"*** — это приложение для составления и управления списком фильмов, которые пользователи планируют посмотреть. Пользователи могут создавать кастомизируемые тематические подборки, что позволяет легко отслеживать интересные фильмы в зависимости от жанров и настроения. Основная цель проекта — предоставить удобный инструмент для организации кинопотока и упрощения поиска подходящих фильмов.

Предметная область включает в себя широкий спектр кинематографических произведений, среди которых пользователи могут выбирать фильмы различных жанров и направлений.

Среди аналогов нашего приложения можно выделить 3 основных: IMDb, Letterboxd и JustWatch. Сравним данные аналоги с нашим приложением по 3 категориям:


| Критерий | Кинопоиск-мини | IMDb | Letterboxd | JustWatch |
|---------------------------|-------------------------------|---------------------------|----------------------------------|---------------------------------|
| Функциональность | Кастомизация тематик, добавление фильмов в список, создание списков на просмотр | Подробные рецензии, трейлеры, рейтинги фильмов | Социальное взаимодействие, оценки фильмов | Поиск фильмов по платформам |
| Пользовательский интерфейс | Интуитивно понятный интерфейс, простой дизайн | Многофункциональный, но иногда загроможденный | Минималистичный и удобный | Простой, но ограниченный функционал |
| Социальные функции | Отсутствуют, акцент на личные списки | Комментарии и рецензии от пользователей | Социальные взаимодействия, друзья, обмен мнениями | Отсутствуют, акцент на функциональности поиска |

Приложение "Кинопоиск-мини" должно обеспечивать следующие функциональные требования:
* фильтровать и сортировать фильмы по различным критериям, таким как жанр или год выпуска;
* возможность пользователям создавать и управлять персонализированными списками фильмов;
* искать фильмы.

### Use-Case диаграмма:
![image](https://github.com/user-attachments/assets/dd9b8080-d481-4ffa-839a-1149a7814c9c)

### ER-диаграмма сущностей (по нотации Чена):
![image](https://github.com/user-attachments/assets/99be4840-2881-4d39-ba26-8b0c1d163c27)

### Пользовательские сценарии:
**Сценарий 1: Фильтрация и сортировка фильмов по жанру**

Цель: Пользователь хочет найти фильмы определенного жанра и отсортировать их по дате выпуска.

Шаги:
1. Пользователь открывает приложение «Кинопоиск-мини».
2. На главном экране пользователь видит панель фильтров и сортировки.
3. Пользователь нажимает на кнопку «Фильтр», чтобы открыть меню фильтрации.
4. Пользователь выбирает жанр, например, «Комедия», из выпадающего списка жанров.
5. После выбора жанра пользователь закрывает меню фильтрации.
6. Пользователь переходит к панели сортировки.
7. Пользователь выбирает сортировку по дате выпуска (от нового к старому).
8. Приложение обновляет список фильмов, показывая только фильмы жанра «Комедия», отсортированные по дате выпуска.
9. Пользователь просматривает отфильтрованные и отсортированные фильмы и выбирает фильм для просмотра подробной информации.

---

**Сценарий 2: Создание и управление персонализированным списком фильмов**

Цель: Пользователь хочет создать новый список фильмов и добавить в него избранные фильмы.

Шаги:
1. Пользователь открывает приложение «Кинопоиск-мини».
2. Пользователь переходит на вкладку «Мои списки» в меню.
3. На экране отображаются уже созданные списки (если есть).
4. Пользователь нажимает на кнопку «Создать новый список».
5. Приложение открывает новый экран для создания списка.
6. Пользователь вводит название списка, например, «Лучшие комедии».
7. Пользователь нажимает кнопку «Сохранить».
8. Новый список появляется на экране «Мои списки».
9. Пользователь переходит в новый список.
10. На экране списка пользователь видит кнопку «Добавить фильм».
11. Пользователь нажимает кнопку «Добавить фильм».
12. Открывается поиск фильмов. Пользователь вводит название фильма.
13. Приложение отображает результаты поиска.
14. Пользователь выбирает фильм из результатов и нажимает кнопку «Добавить».
15. Фильм добавляется в список, и пользователь видит уведомление о успешном добавлении.

---

**Сценарий 3: Поиск фильмов**

Цель: Пользователь хочет найти фильм по названию.

Шаги:
1. Пользователь открывает приложение «Кинопоиск-мини».
2. На главном экране пользователь видит строку поиска вверху.
3. Пользователь кликает по строке поиска.
4. Пользователь вводит название фильма.
5. Приложение отображает результаты поиска в реальном времени, пока пользователь вводит текст.
6. Пользователь видит в результатах как точное совпадение с названием, так и похожие названия.
7. Пользователь находит и выбирает фильм из результатов поиска.
8. Открывается страница с подробной информацией о фильме, включая описание, жанр, год выпуска и рейтинг.


### Экраны будущего web-приложения 
**Главный экран**:

![image](https://github.com/user-attachments/assets/817a69e7-af1f-426c-9f5a-892a2cef42bb)

**Экран со всеми списками фильмов пользователя:**

![image](https://github.com/user-attachments/assets/213de02b-9752-4f3d-9e61-492b940ce185)

**Экран с карточкой фильма:**

![image](https://github.com/user-attachments/assets/05d644eb-f138-4214-98bc-f5b0ade5ea42)

**Экран списка фильмов:**

![image](https://github.com/user-attachments/assets/8f8c9a40-fc50-4921-8d59-b34102b3015e)


