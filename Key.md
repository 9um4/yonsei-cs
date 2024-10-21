# 의미
Relational Database에서 Table 내의 각 Record를 고유하게 식별하기 위한 Attribute 혹은 Attribute의 집합

# 종류
1. Super Key
    - Table 내에서 Row(=Record, Tuple)을 고유하게 식별할 수 있는 하나 이상의 Attribute의 집합
        > `ID`, `(ID, name)` 둘 다 Super Key가 될 수 있음
2. Candidate Key
    - 최소한의 Attribute들로 구성된 Super Key
        > `ID`는 중복이 없는 유일한 값이므로 Candidate Key가 될 수 있음
    - Super Key에서 더 이상 Attribute를 제거할 수 없는 경우
    - Table 내에는 여러 Candidate Key가 존재할 수 있으며, 그 중 하나가 Primary Key로 선택됨
3. Primary Key
    - Table에서 각 Record를 고유하게 식별할 수 있도록 선택된 하나의 Candidate Key
    - 중복이 허용되지 않으며, NULL 값을 가질 수 없음
