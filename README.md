# Setup PostgreSQL container
This GitHub Action loads a PostgreSQL container, allowing you to execute psql commands.

## Usage

```yaml
steps:
- uses: akanieski/setup-postgres-cli@v1
  with:
    # Use any of the binaries that ship with the postgres client (ie. pg_dump, psql, vacuumdb, reindexdb, etc)
    command: |
      pg_dump -U user -h 127.0.0.1 -p 5432 > backup.sql
```
