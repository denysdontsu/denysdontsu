# Denys Dontsu

Python developer focused on backend systems and data pipelines.
I build things that collect, process, and serve data reliably —
and pay attention to what happens between the request and the response.

---

## About

Hands-on experience building REST APIs and ETL pipelines from scratch.
I focus on what happens between input and output — status codes,
validation layers, retry logic, error handling, data consistency.
Not just whether the result looks right, but why it's correct.

---

## Technical Skills

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat&logo=sqlalchemy&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat&logo=postman&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)

| Area | Details |
|---|---|
| APIs & Web | REST, HTTP, status codes, headers, JWT, OAuth2, DevTools (Network tab) |
| Python | FastAPI, SQLAlchemy async, Pydantic v2, requests, BeautifulSoup4 |
| Databases | PostgreSQL, schema design, constraints, indexes, Alembic |
| Tools | Postman, Swagger UI, Git, Linux CLI |
| English | B1 — technical documentation, written communication |

---

## Projects

### 🌍 Language Learning Platform API

Backend REST API with 20+ endpoints covering authentication, exercise delivery, spaced repetition, history tracking, and learning statistics.

- Three-level validation: Pydantic (request), business logic (validators.py), database constraints (CHECK, partial indexes)
- Tested all endpoints via Postman and Swagger UI — including invalid input and edge cases — to verify response behavior and database reactions
- Spaced repetition logic with status-based timeouts: correct (14d), skip (3d), incorrect (immediate retry)

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Status](https://img.shields.io/badge/status-in%20development-yellow)

[→ View repository](https://github.com/denysdontsu/LanguageProject)

---

### 📚 Oxford-Cambridge Vocabulary Builder

Data pipeline that merges Oxford 3000/5000 word lists with CEFR profiles and fetches British IPA transcriptions and audio from Cambridge Dictionary. ~10,300 words processed at ~97% success rate.

- HTTP error handling by response type: 429 → immediate stop; 403 (5x consecutive) → session pause; timeout → retry with backoff up to 5 attempts
- Three-level logging (INFO / WARNING / ERROR) to separate retryable errors from permanent failures
- Incremental saves every 10 words with `--continue` flag for safe resume after interruption

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Status](https://img.shields.io/badge/status-completed-brightgreen)

[→ View repository](https://github.com/denysdontsu/oxford-cambridge-vocabulary-builder)

---

## Contact

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/denys-dontsu)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:dendontsi01@gmail.com)
