# Генератор случайных цитат

Простое веб-приложение на Go, которое отображает случайную цитату, версию приложения и IP-адрес сервера. Сборка и запуск осуществляются с помощью Docker и GitLab CI/CD.

## Структура проекта
- `main.go` — основной исходный код приложения на Go
- `index.html` — HTML-шаблон для отображения цитаты
- `styles.css` — стили для страницы
- `Dockerfile` — инструкция для сборки контейнера
- `docker-compose.yml` — запуск приложения и тестов в контейнерах
- `.gitlab-ci.yml` — CI/CD пайплайн для GitLab

### Тестирование
В docker-compose определён сервис `test`, который проверяет доступность приложения через curl.

### CI/CD
- Сборка, тестирование и публикация образа автоматизированы через `.gitlab-ci.yml`.
- Публикация образа происходит только для ветки `main`.
