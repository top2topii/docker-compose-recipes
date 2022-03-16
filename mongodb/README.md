# mongodb
- mv dotenv .env
- edit .env
- docker-compose up -d
- docker-comnpose down

## Add user(db.createUser)
- mongdb shell
- admin 인증
- 데이터베이스 접근
- 사용자 만들기

## mongodb shell
- docker exec -it docker-mongodb mongo

## db.auth()로 admin 인증
- \> use admin
- \> db.auth('root', 'password')
- \> use test_db
- switched to db test_db
- \> db.createUser({ user: 'dbuser', pwd: 'Secret123', roles:['dbOwner'] })
- Successfully added user: { "user" : "dbuser", "roles" : [ "dbOwner" ] }

### 사용자 Roles 공식 문서
- [Built-In Roles - MongoDB Manual](https://docs.mongodb.com/manual/reference/built-in-roles/)

