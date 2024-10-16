# 의미
Database를 설계하는 과정에서 Entity, Attribute, Relationship 간의 구조를 시각적으로 표현한 diagram

# 표현 방법
1. Entity Set
    - 사각형으로 표현
2. Attribute
    - Entity Set을 표현하는 사각형 안의 List로 표현
    - Primary Key는 밑줄 쳐서 표현
3. Relationship Set
    - 마름모로 표현
    - Relationship Set에 의해 생겨나는 Attribute는 두 개의 Entity Set을 표현하는 사각형 사이에 점선으로 표현
    1. Cardinality
        - 선을 바탕으로 표현
            - directed line(화살표) : 1을 의미
            - undirected line : 다수를 의미
    2. Participation
        - Total Participation
        - Partial Participation

# 예시
![alt](img/Entity-Relationship_Diagram.svg)

`student` 여러 명이 한 명의 `professor`를 `advisor`로서 가질 수 있으며 이에 따라 advise를 시작하는 날짜를 의미하는 `start date`라는 Attribute가 생성됨