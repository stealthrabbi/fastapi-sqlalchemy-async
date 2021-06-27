# Fast-API SQLALchemy Async Example


# Setup

1. Install Docker, Docker-compose, Python 3.8+, Poetry for your O/S.



# Run via Docker
1. Run `docker-compose up` in terminal. This will start the `database` (postgres DB) container and `app` (REST backend app)
1. Browse to http://localhost:8000/docs to use Swagger interface for testing endpoints
1. Create initial user via `api/v1/users/open` endpoint. Response should be a 200 indicatnig it was created.
1. Log in via `api/v1/login/access-token`. Supply email address and password used in account creation in previous step. A token should be available
1. Use `api/v1/login-test-token` to verify your auth token is working. A `200` should be returned.


# local Backend development
1. Run database via `docker-compose up database`
1. Start `poetry shell` 
1. Install python dependencies via `poetry install`.
1. Start uvicorn locally form a `poetry shell`: `uvicorn src.main:app --reload`


# TODO
add tests



