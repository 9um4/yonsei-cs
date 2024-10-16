# 의미
Database에서 하나 이상의 Table로부터 가상 Table을 생성하는 개념

> 실제 Data를 저장하지 않고 기존 Table에 저장된 Data를 조회하는 Query의 결과를 보여줌

# 특징
1. 가상 Table
    - 실제로 Data를 저장하지 않고 `SELECT` Query의 결과를 일종의 Table처럼 보여주는 가상 Object
    - 조회 시마다 해당 Data를 참조하는 방식
2. 기존 Table을 기반으로 생성
    - 하나 이상의 기존 Table에 있는 Data를 기반으로 해 생성
    - 여러 Table의 Data를 `Join`하거나 특정 조건을 걸어 필터링한 데이터를 View로 정의 가능
3. Security
    - 기존 Table의 민감한 정보를 노출하지 않고, 필요한 Data만을 User에게 제공
    - 특정 Column만 보여주거나 특정 조건에 맞는 Entity(Row)만 제공
4. Read Only 또는 Update 가능
    - 대부분의 View는 기존 Table의 Data를 Read만 할 수 있는 Read Only View로 제공됨
    - 특정 조건을 만족하는 경우 View를 바탕으로 Data를 Update 할 수 있음
5. 재사용 가능
    - 자주 사용하는 복잡한 Query를 View로 정의해 재사용 할 수 있음
    - Code의 가독성과 유지보수성이 향상됨

# Syntax
## CREATE
```sql
CREATE VIEW faculty AS
    SELECT id,
           name,
           dept_name
    FROM instructor;
```
