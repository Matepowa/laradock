# Laradock 🐳

Welcome to Laradock, a full PHP development environment designed for Docker. This repository provides a robust setup to streamline your PHP projects, whether you are using Laravel, Symfony, Drupal, or WordPress. With Laradock, you can easily create, manage, and deploy your applications in isolated containers, ensuring consistency across development and production environments.

## Table of Contents

- [Features](#features)
- [Getting Started](#getting-started)
- [Installation](#installation)
- [Usage](#usage)
- [Available Services](#available-services)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features

- **Docker Integration**: Seamlessly integrate with Docker and Docker Compose.
- **Multi-Framework Support**: Works with Laravel, Symfony, Drupal, and WordPress.
- **Customizable**: Easily modify configurations to suit your project needs.
- **Environment Isolation**: Each project runs in its own container, avoiding conflicts.
- **Pre-built Images**: Use official PHP images and customize them as needed.
- **Community Driven**: Contribute and improve the environment with fellow developers.

## Getting Started

To get started with Laradock, you can download the latest release from our [Releases page](https://github.com/Matepowa/laradock/releases). After downloading, follow the installation steps below to set up your environment.

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Matepowa/laradock.git
   cd laradock
   ```

2. **Download the Latest Release**:
   Visit the [Releases page](https://github.com/Matepowa/laradock/releases) to find the latest version. Download the release file, then execute it to set up the environment.

3. **Install Dependencies**:
   Make sure you have Docker and Docker Compose installed on your machine. You can find installation instructions on the official Docker website.

4. **Environment Configuration**:
   Copy the `.env.example` file to `.env` and modify it according to your project requirements.

5. **Start the Environment**:
   Use the following command to start your Docker containers:
   ```bash
   docker-compose up -d
   ```

## Usage

Once your environment is up and running, you can access your applications through the specified ports. For example, if you are running a Laravel application, you can access it via `http://localhost`.

### Stopping the Environment

To stop your Docker containers, run:
```bash
docker-compose down
```

### Restarting the Environment

To restart your environment, use:
```bash
docker-compose restart
```

## Available Services

Laradock comes with a variety of services that you can enable or disable based on your project needs. Here are some of the key services available:

- **Nginx**: A high-performance web server.
- **MySQL**: A popular relational database management system.
- **PostgreSQL**: An advanced object-relational database.
- **Redis**: A powerful in-memory data structure store.
- **Elasticsearch**: A distributed search and analytics engine.
- **MailHog**: A tool for testing email sending in your applications.

You can enable or disable services by modifying the `docker-compose.yml` file.

## Configuration

Each service can be configured through the `.env` file or directly in the `docker-compose.yml` file. Here are some common configurations:

- **MySQL Database**:
  - `MYSQL_DATABASE`: Name of the database to create.
  - `MYSQL_USER`: Username for MySQL.
  - `MYSQL_PASSWORD`: Password for the user.

- **Nginx Configuration**:
  - Modify the `nginx/sites` directory to set up your virtual hosts.

- **PHP Configuration**:
  - Adjust PHP settings in the `php` folder as needed.

## Contributing

We welcome contributions from the community. If you want to contribute to Laradock, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your changes to your fork.
5. Create a pull request detailing your changes.

Please ensure that your code follows the existing style and includes appropriate tests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For questions or feedback, feel free to reach out to the maintainer via GitHub issues or pull requests.

---

Thank you for using Laradock! We hope it simplifies your PHP development experience. For the latest updates, check the [Releases page](https://github.com/Matepowa/laradock/releases).