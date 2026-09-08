### Database:

- Docker command: `docker run --name my-postgres -e POSTGRES_PASSWORD=password -p 5432:5432 -d postgres:18`
- Open psql: `docker exec -it my-postgres psql -U postgres`
- View databases in postgres: `docker exect -it my-postgres psql -U postgres -l`
- View tables in postgres: `docker exec -it my-postgres psql -U postgres -d tms`
- Exit psql: `\q`
- Create db: `CREATE DATABASE tms;`
- Switch db: `\c tms`
- List tables in a db: `\dt`
- Clear terminal screen: `\! clear`
- View columns and data types of a table: `\d tickets`
- View all tickets information: `SELECT * FROM tickets;`
- Reset ticket id sequence: `ALTER SEQUENCE tickets_id_seq RESTART WITH 1;`
