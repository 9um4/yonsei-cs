# 역할
- 대용량 Data Set을 만들거나 Processing 할 때 사용하는 Programming Model

# 구조
1. Data Processing Framework
    - Computer Cluster에서 거대한 Data Set을 분할해 Processing
    - 큰 Computation Task를 작고 Parallelizable task로 쪼갬
2. Key Components
    - Map Phase
    - Shuffle and Sort Phase
    - Reduce Phase

# Components
1. Map Phase
    - Input Data를 중간 형태의 Key-Value 형태로 변경
    - Mapper는 data 뭉치에 대해 이를 수행
2. Shuffle and Sort Phase
    - 중간 Key-Value Data를 정렬하고 그룹화
3. Reduce Phase
    - 그룹화된 Data를 Aggregation 하여 Final OutPut 생성