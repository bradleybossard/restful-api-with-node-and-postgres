### Use docker to spin up a postgres instance (running on port 32768)
docker run --name postgres -e POSTGRES_PASSWORD=123 -d -p 5432 postgres

### Run puppies.sql on the postgres instance
psql --user postgres --host 0.0.0.0 --port 32768 --file puppies.sql
