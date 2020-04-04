# SpringBoot

docker run --name postgres-spring -e POSTGRES_PASSWORD=abc123 -d -p 5432:5432 postgres:alpine

docker exec -it db70dbc39f73 bin/bash

psql -U postgres

CREATE DATABASE demodb;

\l

\c demodb

\d

\dt

CREATE EXTENSION "uuid-ossp";
SELECT uuid_generate_v4();
INSERT INTO person(id,name) VALUES (uuid_generate_v4(), 'Maria Jones');