# 의미
Database의 구조를 정의하는 언어

# 예시
```sql
create table instructor(
    ID          char(5),
    name        varchar(20),
    dept_name   varchar(20),
    salary      numeric(8,2)
)
```
- instructor table을 생성하는 SQL 구문
- `data dictionary` 혹은 `system catalogue`라고 부르는 Database의 System과 관련한 Table을 변경하는 작업도 수행