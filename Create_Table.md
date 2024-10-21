# 의미
Table을 생성하기 위한 구문

# 문법
```sql
create table <table name> (
    <attribute name 1>  [<domain of attribute 1>]   [<constraint of attribute 1>],
    ...,
    <attribute name n>  [<domain of attribute n>]   [<constraint of attribute n>],
    [integrity constraints 1],
    ...
    [integrity constraints n]
)
```

# 용례
```sql
create table instructor (
    ID              char(5),
    name            varchar(20)                         not null,
    dept_name       varchar(20)                         not null,
    salary          numeric(8, 2),
    primary key     (ID),
    foreign key     (dept_name) references department
);
```

```sql
create table takes (
    ID          varchar(5),
    course_id   varchar(8),
    sec_id      varchar(8),
    semester	varchar(6),
    year		numeric(4,0),
    grade		varchar(2),
    primary key	(ID, course_id, sec_id, semester, year),
    foreign key	(ID) references student,
    foreign key	(course_id, sec_id, semester, year) references section
);
```

```sql
CREATE TABLE orders (
    order_id        int     PRIMARY KEY,
    customer_id     int,
    foreign key (customer_id) REFERENCES customers(customer_id)
    ON DELETE CASCADE
);
```