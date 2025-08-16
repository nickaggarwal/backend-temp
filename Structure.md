project-name/
├── app/
│   ├── __init__.py
│   ├── main.py                 # FastAPI app initialization & configuration
│   ├── config.py                # Settings and environment variables
│   │
│   ├── api/                     # API endpoints
│   │   ├── __init__.py
│   │   ├── v1/
│   │   │   ├── __init__.py
│   │   │   ├── endpoints/
│   │   │   │   ├── __init__.py
│   │   │   │   ├── users.py
│   │   │   │   ├── auth.py
│   │   │   │   └── items.py
│   │   │   └── router.py       # Main API router
│   │   └── dependencies.py      # Shared dependencies
│   │
│   │
│   ├── models/                  # Database models
│   │   ├── __init__.py
│   │   ├── user.py
│   │   └── item.py
│   │
│   ├── schemas/                 # Pydantic models/schemas
│   │   ├── __init__.py
│   │   ├── user.py
│   │   └── item.py
│   │
│   ├── services/               # Business logic
│   │   ├── __init__.py
│   │   ├── user_service.py
│   │   └── item_service.py
│   │
│   ├── utils/                  # Utility functions
│   │   ├── __init__.py
│   │   └── helpers.py
│
├── tests/                      # Test files
│   ├── __init__.py
│   ├── conftest.py            # Pytest fixtures
│   ├── test_api/
│   │   └── test_users.py
│   └── test_services/
│       └── test_user_service.py
│
├── migrations/                 # Database migrations (Alembic)
│   └── alembic.ini
│
├── docker/                     # Docker-related files
│   ├── Dockerfile
│   └── docker-compose.yml
│
├── .env.example               # Example environment variables
├── .gitignore
├── requirements.txt           # Production dependencies
├── requirements-dev.txt       # Development dependencies
├── README.md
└── pyproject.toml            # Project configuration (if using Poetry)
