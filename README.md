# Renovate Test API

Simple FastAPI application to test Renovate dependency updates.

## Dependencies (outdated on purpose)

- FastAPI 0.68.0
- Uvicorn 0.14.0
- Pydantic 1.8.2

## Run locally

```bash
pip install -r requirements.txt
uvicorn main:app --reload
```

## Run with Docker

```bash
docker build -t renovate-test .
docker run -p 8000:8000 renovate-test
```

## API Endpoints

- `GET /` - Hello World
- `GET /health` - Health check
- `GET /items/{item_id}` - Get item by ID
