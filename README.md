# Laravel Articles

A Laravel blog for listing, creating, showing, editing, and deleting articles.

## Routes

- `GET /home` shows the home page
- `GET /articles` lists articles
- `GET /article/create` shows the create form
- `POST /articles` stores a new article
- `GET /articles/{article}` shows one article
- `GET /articles/{article}/edit` shows the edit form
- `PATCH /articles/{article}` updates an article
- `DELETE /articles/{article}` deletes an article

## Tech Stack

- PHP ^8.0.2
- Laravel 9
- Blade
- MySQL

## Requirements

- PHP ^8.0.2
- Composer
- MySQL

## Installation

```bash
composer install
cp .env.example .env
php artisan key:generate
```

Create a MySQL database, then set these values in `.env`:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=laravel
DB_USERNAME=root
DB_PASSWORD=
```

Then run:

```bash
php artisan migrate
php artisan serve
```

Open `http://localhost:8000/home`.

The `employees` migration creates a table with `name`, `image`, `email`, `password`, and `status`.
