# GraphQL Project 🐬

## О проекте

Это проект с использованием Django и GraphQL, который позволяет выполнять запросы для получения данных о пользователях.

## Установка

1. Клонируйте репозиторий:

```bash
git clone https://github.com/твой_никнейм/имя_репозитория.git
```
2. Установите зависимости:
```bash
pip install -r requirements.txt
```
3. Выполните миграции:
```bash
python manage.py migrate
```
4. Запустите сервер:
```bash
python manage.py runserver
```
## Примеры запросов GraphQL
### Получение всех пользователей:
{
  allUsers {
    id
    username
    email
  }
}
### Получение одного пользователя по ID:
query GetUser($id: ID!) {
  user(id: $id) {
    name
    age
    id
  }
}
