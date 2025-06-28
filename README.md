# 📚 Book Review API

A simple and efficient backend API for managing books and their reviews. Built using **FastAPI**, **SQLAlchemy**, and **SQLite**, with basic caching and test coverage.

---

## 🚀 Features

- Add and list books
- Add and list reviews for each book
- Simple in-memory caching for review data
- Modular architecture (CRUD, models, schemas)
- Pytest-based unit tests

---

## 🧰 Tech Stack

- **Framework**: FastAPI
- **ORM**: SQLAlchemy
- **Database**: SQLite
- **Cache**: In-memory dictionary (mock Redis)
- **Testing**: Pytest
- **Server**: Uvicorn (ASGI)

---

## 📦 Installation

## Create and activate virtual environment

python -m venv venv
source venv/bin/activate # On Windows: venv\Scripts\activate

## Install dependencies

pip install -r requirements.txt

## Running the Server

uvicorn main:app --reload

Visit: http://127.0.0.1:8000

Swagger Docs: http://127.0.0.1:8000/docs

Redoc: http://127.0.0.1:8000/redoc

## Run Tests

pytest

## Project Structure

Project/
│
├── main.py # Entry point with all routes
├── models.py # SQLAlchemy models
├── schemas.py # Pydantic models for validation
├── crud.py # Business logic (Create, Read)
├── database.py # DB engine and session setup
├── cache.py # In-memory cache for reviews
├── test_main.py # Pytest unit tests
├── requirements.txt # Project dependencies
└── README.md # Project documentation
