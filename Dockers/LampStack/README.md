# Docker Compose PHP Project

This project sets up a development environment using Docker Compose with PHP, Apache, MySQL, and phpMyAdmin. Below are the instructions to get started.

## Project Structure

```
docker-compose-php-project
├── docker-compose.yml
├── .env
├── php
│   ├── Dockerfile
│   └── src
│       └── index.php
├── mysql
│   └── data
└── README.md
```

## Prerequisites

- Docker
- Docker Compose

## Setup Instructions

1. **Clone the repository** (if applicable):
   ```
   git clone <repository-url>
   cd docker-compose-php-project
   ```

2. **Create a `.env` file**:
   Update the `.env` file with your database credentials and other configuration settings.

3. **Build and start the services**:
   Run the following command in the project root directory:
   ```
   docker-compose up -d
   ```

4. **Access the application**:
   Open your web browser and navigate to `http://localhost:8080` to see the PHP application running.

5. **Access phpMyAdmin**:
   You can access phpMyAdmin at `http://localhost:8081` to manage your MySQL databases.

## Stopping the Services

To stop the running services, use:
```
docker-compose down
```

## Notes

- The MySQL data is stored in the `mysql/data` directory to ensure data persistence.
- The PHP application can be modified in the `php/src/index.php` file.

## License

This project is licensed under the MIT License.