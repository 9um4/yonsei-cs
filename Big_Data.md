# 정의
  - 전통적인 Data Processing Application들이 처리하기 어려운 대규모 복잡 Data Set
  - Social Media, Sensor, Transaction 등 다양한 소스에서 기하급수적으로 증가

# 특성
  1. Volume : 방대한 Data 규모
  2. Velocity : 빠른 Data 생성 속도, Real-time Processing 필요
  3. Variety : Structured, Semi-Structured, Unstructured Data Format 포함

# Efficient Data Storage
1. HDFS (Hadoop Distributed File System)
    - Distributed File System으로서 대규모 Data Set을 Cluster에 분산 저장
2. NoSQL
    - 유연한 Data Model과 높은 Scalability 제공
    - MongoDB, Cassandra

# Data Processing
1. Batch Processing
    - 일정 주기마다 Data의 대규모 Processing을 처리
    - 즉각적으로 insight가 필요하지 않은 경우에 이용
    - 금융 서비스, Data Warehousing 등등
2. Real-time Processing
    - 실시간으로 Data를 Processing하여 즉각적인 insight 반환
    - 동적인 응답을 요구하는 Application에 사용됨
    - Social Media, Online Platform 등등
3. MapReduce & Spark
    - Distributed Processing으로 Parallel Computation 제공
    - Cluster 간의 병렬 연산
    - Social Network Graph, ML, ETL 등등

# Optimization
1. Scalability
    - 수평적 확장으로 Data 증가를 대처해야 함
2. Availability
    - Data와 System의 높은 가용성 보장
3. Data Partitioning
    - Parallel Processing을 위한 Data Partitioning을 통해 Processing Time 감소
4. Caching
    - 자주 접근하는 Data를 Cache에 저장해 Performance 향상
