# Project Title

This is a PHP project with Docker support. It uses Apache server with SSL enabled.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

You need to have Docker installed on your machine. You can download Docker from [here](https://www.docker.com/products/docker-desktop).

### Installing

1. Clone the repository to your local machine.

2. Navigate to the project directory.

3. Generate SSL keys:

```sh
openssl req -x509 -new -out mycert.crt -keyout mycert.key -days 365 -newkey rsa:4096 -sha256 -nodes
```

4. Build the Docker image:

```sh
docker-compose build
```

5. Run the Docker container:

```sh
docker-compose up
```

The application will be accessible at `https://localhost:8443`.

## Built With

- [PHP](https://www.php.net/)
- [Apache](https://httpd.apache.org/)
- [Docker](https://www.docker.com/)

## Authors

- Mike

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.

## Acknowledgments

- Hat tip to anyone whose code was used
- Inspiration
- etc.
