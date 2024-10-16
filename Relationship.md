# 의미
Database에서 두 개 이상의 Entity 간의 연관성을 나타냄

# 특징
1. Entity 간의 연결
2. Cardinality
3. Relationship 또한 Attribute를 가질 수 있음

# 예시
1. 학생(Entity)와 강의(Entity) 간의 Relationship
    - Relationship : `학생이 강의를 수강함`
    - Cardinality
        - 한 학생이 여러 강의를 들을 수 있고, 한 강의를 여러 학생이 수강할 수 있으므로 `Many to many` Relationship이 성립
    - Attribute : `성적`
2. 교수(Entity)와 강의(Entity) 간의 Relationship
    - Relationship : `교수가 강의를 가르침`
    - Cardinality
        - 한 명의 교수가 여러 강의를 진행할 수 있으므로 `One to many` Relationship이 성립
    - Attribute : 없음