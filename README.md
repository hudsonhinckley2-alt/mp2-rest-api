# MP2 REST API

A FastAPI application that uploads CSV datasets, stores them in memory, and processes them using my reusable MP1 data pipeline. `GET /health` reports the API status, `POST /upload` stores a CSV and returns its metadata, `GET /datasets/{id}` returns stored rows, and `POST /datasets/{id}/process` validates and cleans a dataset and returns a cleaning report. Middleware logs every request with a unique request ID, status code, and duration, and the API is tested with pytest and TestClient.
