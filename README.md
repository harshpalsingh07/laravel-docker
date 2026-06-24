# laravel-docker

## Run the project with Docker

1. Build and start the containers:
    ```bash
    docker compose up -d --build
    ```
2. Open the app in your browser:
    ```text
    http://localhost:8080/
    ```
3. If the app needs dependencies installed inside the container, run:
    ```bash
    docker compose exec app composer install
    ```
4. To generate the Laravel application key:
    ```bash
    docker compose exec app php artisan key:generate
    ```

The stack includes:

- PHP + Laravel app container
- Nginx web server
- MySQL database container
