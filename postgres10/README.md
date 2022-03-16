# PostgreSQL 10
- https://evergrow.tistory.com/42

## 설치후 한 일
- dbuser 생성
```sh
docker exec -it postgres10 /bin/sh
su - postgres
psql

postgres=# CREATE USER userid with PASSWORD 'password' CREATEDB;
postgres=# CREATE DATABASE testdb;
postgres=# \c testdb;
postgres=# GRANT ALL PRIVILEGES ON DATABASE testdb TO dbuser;

```

