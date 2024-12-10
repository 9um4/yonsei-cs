# 의미
- 특정 Transaction Set의 Serializability를 확인 하기 위해 사용되는 Direct Graph
- 각 Vertex는 하나의 Transaction을 나타냄
- 각 Arc는 두 Transaction 간의 Conflict 관계를 나타냄

# 구성
- Transaction 간 충돌: Arc
  - 먼저 실행된 Transaction에서 이후 실행된 Transaction으로 방향성 있는 연결

# Serializability 확인
- Acyclic Graph
- Acyclic 한 경우 Topological Sorting을 통해 Serial Execution 순서 도출 가능