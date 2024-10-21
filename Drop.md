# 의미
Table, Database View, Index, Trigger 같은 Database 객체를 완전히 삭제

# 구문
```sql
drop <object type> <table name>
```

> Object Type에는 `Table`, `Database`, `View`, `Index`, `Trigger` 등이 있음

```sql
drop <object type> <table name> cascade;
```

> `cascade` 사용시 연관된 모든 Table(foreign key 기준) 삭제