Title: Add persistent storage and domain models for activities, students, and users

Description:
Replace the current in-memory `activities` store with a persistent database and implement typed domain models for Activities, Students, and Users. This will enable data durability, queries, and future migrations.

Acceptance criteria:
- Add a database dependency and configuration for SQLite (dev) and Postgres (production).
- Introduce models (ORM/Pydantic/SQLModel) for Activity, Student, User with fields used in the app.
- Update API endpoints to persist and read from the DB instead of the in-memory dict.
- Include database migration instructions or simple migration tooling (e.g., Alembic or SQLModel create_all).
- Tests for basic CRUD for activities and participants.

Suggested tasks:
- Add `src/models.py` with Activity/Student/User models.
- Add `src/db.py` for DB session management and init.
- Update `src/app.py` endpoints to use DB session.
- Add tests in `tests/test_db_models.py`.

Priority: High
Estimate: 2-3 days
