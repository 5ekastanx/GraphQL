<div style="text-align: center;"><h1 style="text-align: center;">GraphQL Project 🐬</h1></div>

## О проекте

Это проект с использованием Django и GraphQL, который позволяет выполнять запросы для получения данных о пользователях.

## Установка

1. Клонируйте репозиторий:

```bash
git clone https://github.com/5ekastanx/GraphQL.git
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
  users {
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
