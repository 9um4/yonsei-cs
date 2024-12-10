# 정의
대규모 File을 작은 block으로 나누고 다중 node에 저장

# 구조
1. Data Distribution
    - HDFS의 Data는 Block이라 부르는 작은 덩어리로 나뉨
    - Cluster 내의 다중 node들에 분산됨
    - Parallel Processing과 Efficient Storage Management를 가능케 함
2. Key Components
    1. Name Node : File System의 Metadata 관리 및 저장
    2. Data Node
        - 실제 Data Block 저장
        - 주기적으로 Name Node에 상태와 저장하는 Block에 대해 보고
3. Resilience
    - Data Replication에 대한 Scalability와 Fault Tolerance 달성