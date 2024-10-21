# 의미
Data를 행(Row), 혹은 튜플(Tuple)과 열(Column) 또는 속성(Attribute) 구성하는 Table

# 수학적 정의
1. 집합 $\rm D_1, ~ D_2, ~ \cdots ~ , D_n$에 대해서 Relation $r$은 $\rm D_1 \times D_2 \times \cdots \times D_n$의 subset
2. Relation Schema $R$에 대해 $r(R)$은 $R$에 대한 Relation

# 구성 요소
1. 행(Row), 튜플(Tuple)
    - 각 Row(Tuple)은 하나의 Record를 나타냄
    - Table에 정의된 Attribute의 값을 가지고 있음
        > 학생 Table에서 하나의 Row는 한 명의 학생에 대한 정보를 나타냄
1. 열(Column), 속성(Attribute)
    - 특정한 데이터 항목을 의미
    - Table의 구조를 정의하고, 각 Tuple이 가질 수 있는 값을 결정
        > 학생 Table에서 `학번`, `이름`, `전공`과 같은 것
2. 도메인(Domain)
    - 각 Attribute가 가질 수 있는 값의 범위
        > `나이` Attribute는 양의 정수의 Domain을 가짐
3. 카디널리티(Cardinality)
    - Table에 있는 Row(Tuple)의 수
4. 차수(Degree, Arity)
    - Table에 있는 Column(Attribute)의 수

# 특징
1. 순서가 없는 Tuple
2. 순서가 없는 Attribute
3. 중복이 없는 Tuple