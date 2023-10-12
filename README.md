
# elect-archive

laravelを利用して作成

```bash
sudo apt install postgresql
sudo -i -u postgres
psql
ALTER USER postgres with encrypted password 'postgres';
exit;exit;
sudo nano /etc/postgresql/14/main/pg_hba.conf 
peer→md5
sudo service postgresql restart
```

```php
laravel new elect-archive
composer require laravel/breeze
php artisan breeze:install blade
php artisan migrate
npm install
npm run dev
```

```
```
