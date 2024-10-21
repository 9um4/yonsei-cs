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

# 기능 (지정할 수 있는 것들)
- The schema for each relation

    ```sql
    CREATE TABLE students (
        student_id      int,
        name            varchar(20),
        age             int
    )
    ```
- The domain of values associated with each attribute
    > `INT`, `VARCHAR`, `NUMERIC`과 같은 Data Type을 이용해 Domain 정의
- Integrity Constraints
    ```sql
    CREATE TABLE students (
        student_id      int             PRIMARY KEY,
        name            varchar(20)     NOT NULL,
        age             int             CHECK (age >= 18)
    )
    ```
- The set of indices to be maintained for each relation
    ```sql
    CREATE INDEX idx_name ON students (name)
    ```
- Security and authorization information for each relation
    ```sql
    GRANT SELECT ON students TO user1;
    ```
- The physical storage structure of each relation on disk