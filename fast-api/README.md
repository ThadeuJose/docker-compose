## Compose sample application

### Python/FastAPI application

Project structure:

```
├── docker-compose.yaml
├── Dockerfile
├── requirements.txt
├── app
    ├── main.py
    ├── __init__.py

```

## Deploy with docker compose

```
docker compose up -d --build
```

## Expected result

Listing containers must show one container running and the port mapping.

After the application starts, navigate to `http://localhost:8000` in your web browser and you should see the following json response:

```
{
  "message": "OK"
}
```

## Stop and remove the containers

```
docker compose down
```
