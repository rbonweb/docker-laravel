Commands to run the project of laravel with docker

[]: # Clone the project
git clone

[]: # Install dependencies
docker-compose exec app composer install

[]: # Create .env file
docker-compose exec app cp .env.example .env

[]: # Generate key
docker-compose exec app php artisan key:generate

[]: # Run migrations
docker-compose exec app php artisan migrate

[]: # Run seeders
docker-compose exec app php artisan db:seed

[]: # Run tests
docker-compose exec app php artisan test

[]: # Run optimize
docker-compose exec app php artisan optimize