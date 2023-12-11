# toedoe-list-api

A laravel learning project, working as the API for my [toedoe-list-vue](https://github.com/0xAlMo3geZ/toedoe-list-vue) learning project.

## Installation

1. Download the code by clicking **Code**, **Download ZIP**. Or if you have Git install in your machine, you can run this in your terminal.

```
git clone https://github.com/0xAlMo3geZ/toedoe-list-api.git
```

2. Change directory to your local copy of `toedoe-list-api` in your terminal. Then install composer dependencies.

```
composer install
```

3. Copy `.env` file from `.env.example`. In NIX machine you can use this command.

```
cp .env.example .env
```

4. Prepare a database. You can use this command.

```
mysql -uroot -e "CREATE DATABASE toedoe-list-api-db"
```

If you have password for your database, you need to specify `-p` on the command.

5. Configure your database settings in `.env`

```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=toedoe-list-api-db
DB_USERNAME=root
DB_PASSWORD=
```

6. Migrate database tables and seed them with fake data

```
php artisan migrate --seed
```

7. Generate a key for you application

```
php artisan key:generate
```

8. Install frontend dependencies.

```
npm install
```

9. Run local server

```
php artisan serve
```

Your local copy of toedoe-list-api is ready to access in your browser ;)
