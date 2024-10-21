# 의미
Table에 새로운 Row(Record, Tuple)을 Insert하는데 사용하는 SQL 구문

# 구문
## 모든 Attribute에 상응하는 값을 가지고 있는 Tuple
```sql
insert into <table name> values (
    <attribute 1 value>,
    ...,
    <attribute n values>
);
```

## 특정 Attribute에만 상응하는 값을 가지고 있는 Tuple
```sql
insert into <table name> (
    <attribute 1 name>,
    ...,
    <attribute n name>
)
values (
    <attribute 1 value>,
    ...,
    <attribute n value>
);
```

## 여러 Row(Record, Tuple) 삽입
```sql
insert into <table name> (
    <attribute 1 name>,
    ...,
    <attribute n name>
)
values (
    <attribute 1 value>,
    ...,
    <attribute n value>
),
(
    <attribute 1 value>,
    ...,
    <attribute n value>
),
...,
(
    <attribute 1 value>,
    ...,
    <attribute n value>
);
```

# 용례
```sql
insert into instructor values (
    '10211',
    'Smith',
    'Biology',
    66000
)
```