# WordPress Docker Setup

## Overview

This project provides a Docker-based setup for a WordPress development environment. It includes services for WordPress, MySQL, phpMyAdmin, and WP-CLI, with auto-configuration capabilities.

## Prerequisites

- Docker
- Docker Compose

## Features

- WordPress installation with auto-configuration
- MySQL database
- phpMyAdmin for database management
- WP-CLI for command-line management of WordPress
- Health check for service availability

## Setup

1. **Clone the repository:**

   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. **Environment Configuration:**

   Customize environment variables in the `wp-auto-config.yml` and `docker-compose.yml` files to suit your setup.

3. **Build and Start Services:**

   Run the following command to build and start the services:

   ```bash
   make install
   ```

   This will start the WordPress and MySQL services, perform health checks, and apply WordPress auto-configuration.

4. **Access WordPress:**

   Open your web browser and navigate to `http://localhost` to access your WordPress site.

5. **Access phpMyAdmin:**

   Access phpMyAdmin at `http://localhost:<PHPMYADMIN_PORT>` for database management.

## Makefile Commands

- `start`: Build and start the Docker containers
- `healthcheck`: Run health checks for services
- `down`: Stop and remove containers
- `install`: Start services and perform health checks
- `configure`: Run WordPress auto-configuration
- `autoinstall`: Start services and run auto-configuration
- `clean`: Remove related files and folders
- `reset`: Clean the setup

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
