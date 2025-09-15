# grthomson/docker-rust-postgres

Minimal Rust + PostgreSQL service (Actix Web).

## Usage
```bash
docker pull grthomson/docker-rust-postgres:latest
docker run -p 8000:8000 \
  -e PG_HOST=host.docker.internal \
  -e PG_DBNAME=example \
  -e PG_USER=postgres \
  -e PG_PASSWORD=mysecretpassword \
  grthomson/docker-rust-postgres:latest
  ```

## Endpoints

```GET /users```, ```GET /healthz```