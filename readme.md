# E-Service System

A service management web application built with **Laravel**, **Vue.js** and **Inertia.js**. It supports role-based access (manager and employee), applicant management, system users and pricing.

## Features

- Role-based access: manager and employee roles, assignable from the Users section
- Applicants (certified users) management
- System users management
- Price list management

## Tech stack

- PHP, Laravel
- Vue.js, Inertia.js
- Tailwind CSS, Laravel Mix
- SQLite / MySQL / PostgreSQL

## Getting started

```bash
git clone https://github.com/Imranali2726/e-service.git
cd e-service
composer install
npm install
npm run dev
cp .env.example .env
php artisan key:generate
```

Set the mail driver in `.env` to `log` (or use Mailhog) for local development.

Create a database. SQLite is the quickest; for MySQL or PostgreSQL, update `.env` instead.

```bash
touch database/database.sqlite
php artisan migrate --seed
php artisan serve
```

## Demo accounts (local seed data)

| Role | Email | Password |
| --- | --- | --- |
| Manager | admin@example.com | 12345678 |
| Employee | employee@example.com | 12345678 |

## Main pages

- Applicants: `/certified-users`
- System users: `/users`
- Prices: `/prices`

## License

MIT
