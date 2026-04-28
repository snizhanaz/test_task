# SQL Test Task (PostgreSQL)

## Task
Отримати список користувачів (ім’я + прізвище), які зареєструвалися за останні 30 днів.

## Solution
```sql
SELECT first_name, last_name
FROM users
WHERE creation_date >= CURRENT_DATE - INTERVAL '30 days';
