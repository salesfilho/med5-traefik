# med5-docker-traefik

This project sets up a development environment using Docker and Traefik for the `med5` application.

## Prerequisites

- [Docker](https://docs.docker.com/get-docker/) installed
- [Docker Compose](https://docs.docker.com/compose/install/) installed

```
# Instale o apache2-utils se não tiver (Linux)
sudo apt-get install apache2-utils

# Crie o hash de usuário e senha (substitua 'usuario' e 'senha' pelos seus valores)

htpasswd -nb usuario senha
````



## Project Structure

```
med5-docker-traefik/
├── docker-compose.yml
├── traefik/
│   ├── traefik.yml
│   └── acme.json
├── app/
│   └── ... (your application files)
└── readme.md
```

## Usage

1. **Clone the repository:**
    ```bash
    git clone https://github.com/yourusername/med5-docker-traefik.git
    cd med5-docker-traefik
    ```

2. **Configure environment variables:**  
    Edit `.env` or relevant config files as needed.

3. **Start the services:**
    ```bash
    docker-compose up -d
    ```

4. **Access your application:**  
    Open your browser and go to [http://localhost](http://localhost) or the configured domain.

## Traefik Dashboard

- The Traefik dashboard is available at [http://localhost:8080](http://localhost:8080) by default.

## Customization

- Modify `docker-compose.yml` to add or change services.
- Edit `traefik/traefik.yml` for Traefik configuration.

## Stopping the Environment

```bash
docker-compose down
```

## License

MIT License

---

*Replace placeholders and paths as needed for your specific setup.*