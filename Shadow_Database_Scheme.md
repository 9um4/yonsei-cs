# 의미
- 오직 1개의 Transaction이 한 번에 Active됨
- DB_Pointer가 항상 Database의 사본을 가리킴
- 모든 Update는 Shadow Copy에서 수행됨
- Transaction을 실패할 경우 기존 db_pointer를 사용
- 대규모 Database에서는 비효율적