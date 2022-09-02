![example workflow](https://github.com/Komappp/yamdb_final/.github/workflows/yamdb_workflow.yml/badge.svg)
![example workflow](https://github.com/github/docs/actions/workflows/yamdb_workflow.yml/badge.svg)
# Проект YaMDb

Проект YaMDb собирает отзывы (Review) пользователей на произведения. 
Произведения делятся на категории: «Книги», «Фильмы», «Музыка». Список категорий может быть расширен администратором.
Произведению может быть присвоен жанр из списка предустановленных.
Новые жанры может создавать только администратор.

Пользователи оставляют к произведениям текстовые отзывы и ставят произведению оценку в диапазоне от одного до десяти.
Из пользовательских оценок формируется усреднённая оценка произведения — рейтинг.
На одно произведение пользователь может оставить только один отзыв.

# Ресурсы API YaMDb
**AUTH**: аутентификация.

**USERS**: пользователи.

**TITLES**: произведения, к которым пишут отзывы (определённый фильм, книга или песенка).

**CATEGORIES**: категории (типы) произведений ("Фильмы", "Книги", "Музыка").

**GENRES**: жанры произведений. Одно произведение может быть привязано к нескольким жанрам.

**REVIEWS**: отзывы на произведения. Отзыв привязан к определённому произведению.

**COMMENTS**: комментарии к отзывам. Комментарий привязан к определённому отзыву.

# Установка
Склонируйте репозиторий. Создайте виртуальное окружение, активируйте его.

Для запуска сервера разработки,  находясь в директории проекта выполните команды:
```
python manage.py migrate
python manage.py createsuperuser
python manage.py collectstatic --no-input
python manage.py runserver
```
 
