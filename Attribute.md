# 의미
Database에서 Entity가 가지는 특성이나 정보를 나타내는 element

# 특징
1. Entity를 설명함
    - Entity가 가지고 있는 구체적인 정보를 나타냄
    - Database에서 저장하고 관리해야 하는 실제 Data
2. Entity를 고유하게 식별하기 위한 Primary Key로 사용될 수 있음
    - Primary Key는 고유해야 함

# 유형
1. Simple Attribute
    - 더 이상 나눌 수 없는 단일 값을 가진 Attribute
    - 예시) 학번
2. Composite Attribute
    - 여러 Attribute로 나눌 수 있는 Attribute
    - 예시) 주소
        - 도, 시, (구), 길, 번지로 나뉠 수 있음
3. Single-valued Attribute
    - 하나의 Entity가 한 개의 값을 가질 수 있는 Attribute
    - 예시) 생년월일
4. Multivalued Attribute
    - 하나의 Entity가 여러 개의 값을 가질 수 있는 Attribute
    - 예시) 이메일 주소
5. Derived Attribute
    - 다른 Attribute로 계산되어 나오는 Attribute
    - 예시) 나이
        - 생년월일을 통해 계산됨