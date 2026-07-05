Title: Add Docker and deployment manifests

Description:
Add Dockerfile(s) and `docker-compose.yml` for local development and simple deployment. Provide instructions to run the app with persistent DB in Docker.

Acceptance criteria:
- Add `Dockerfile` for the FastAPI app and service in `docker-compose.yml`.
- Configure a database service (Postgres) in `docker-compose.yml` and networking.
- Document `docker-compose up` steps in `README.md`.

Suggested tasks:
- Add `Dockerfile` and update `README.md` with Docker instructions.
- Add example `.env.example` with DB connection settings.

Priority: Medium
Estimate: 1 day
