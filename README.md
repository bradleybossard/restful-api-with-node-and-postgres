# Designing a RESTful API With Node and Postgres 

### Link to original blog post
[Designing a RESTful API With Node and Postgres - Michael Herman](http://mherman.org/blog/2016/03/13/designing-a-restful-api-with-node-and-postgres/#.WekuchNSxTZ)

### Use docker to spin up a postgres instance (running on port 32768)
`docker run --name postgres -e POSTGRES_PASSWORD=123 -d -p 5432 postgres`

### Run puppies.sql on the postgres instance
`psql --user postgres --host 0.0.0.0 --port 32768 --file puppies.sql`
