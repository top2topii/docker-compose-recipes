# PostgreSQL 10
- https://evergrow.tistory.com/42

## 설치후 한 일
- dbuser 생성
```sh
docker exec -it postgres10 /bin/sh
su - postgres
psql

postgres=# CREATE USER db_userid with PASSWORD 'password' CREATEDB;
postgres=# CREATE DATABASE db_name;
postgres=# \c db_name;
postgres=# GRANT ALL PRIVILEGES ON DATABASE db_name TO db_userid;

```

## psql 몇가지 명령
- 접속: 
```sh
psql -U db_userid
```
- database 조회: 
```sh
postgres=# \l
```
- user 조회: 
```sh
postgres=# \du
```
- database 접속:
```sh
postgres=# \c db_name
```
- 소유자 변경:
```sh
postgres=# ALTER DATABASE db_name OWNER TO db_userid;
```
