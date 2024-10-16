# 의미
Entity-Relationship Model의 Entity, Attribute, Relationship을 Relational Database의 Schema로 변환하는 과정

# 필요성
이 과정을 바탕으로 Entity-Relationship Model로 설계된 Database Model을 Relational Database로 실제 구현할 수 있음

# 특징
각각의 Schema는 Attribute의 개수에 해당하는 만큼의 유일한 이름의 Column을 가지게 됨

# 단계
1. Entity Set을 하나의 Table로 변환
    - 각 Entity Set은 하나의 Table로 변환됨
    - 각 Entity의 Attribute는 Table의 Column이 됨
    - 각 Entity의 Primary Key는 Table의 Primary Key가 됨
2. Relationship Set을 하나의 Table로 변환
    1. One to one : 각 Entity의 Primary Key를 서로 참조하도록 하여 하나의 Table에 Relationship을 저장할 수 있음
    2. One to many : Many에 해당하는 Entity가 One에 해당하는 Entity의 Primary Key를 Foreign Key로 참조하도록 하여 Relationship을 표현할 수 있음
    3. Many to many : 각 Entity의 Primary Key를 참조하는 별도의 Join Table을 생성하여 Relationship을 표현할 수 있음
3. Attribute의 표현
    - 각 Entity와 Relationship의 Attribute들이 Table의 Column으로 변환됨
    - Composite Attribute는 여러 개의 Single Attribute로 나뉘어지고, Multi-valued Attribute는 별도의 Table로 변환될 수 있음