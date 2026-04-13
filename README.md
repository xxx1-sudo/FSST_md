# Velox API

**A lightweight REST API built with FastAPI**

![Python 3.11+](https://img.shields.io/badge/Python-3.11%2B-blue?logo=python)
![FastAPI 0.111](https://img.shields.io/badge/FastAPI-0.111-009688?logo=fastapi)
![License MIT](https://img.shields.io/badge/License-MIT-green)

---

A minimal REST API for user authentication and resource management. No unnecessary dependencies, no bloat.

## Installation

```bash
git clone https://github.com/yourname/velox-api.git
cd velox-api
pip install -r requirements.txt
uvicorn app.main:app --reload
```

API runs at `http://localhost:8000` · Docs at `/docs`

## Endpoints

| Method | Endpoint      | Description       |
|--------|---------------|-------------------|
| POST   | `/auth/login` | Obtain JWT token  |
| GET    | `/users/me`   | Get current user  |
| GET    | `/items/{id}` | Retrieve item     |
| POST   | `/items`      | Create item       |

## Project Structure

```
velox-api/
├── app/
│   ├── main.py          # Entry point
│   ├── routers/         # Route definitions
│   ├── models/          # Database models
│   └── schemas/         # Pydantic schemas
└── requirements.txt
```

## Contributing

Fork → branch → commit → pull request. Issues welcome.
