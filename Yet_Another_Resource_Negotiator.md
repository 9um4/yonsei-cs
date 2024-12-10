# 역할
- 자원 관리 및 Task Scheduling 담당
- 동적으로 Memory와 CPU를 다른 Application에 할당

# 구조
1. Resource Management
    - 효율적으로 Cluster Resource를 할당
2. Key Components
    - ResourceManager : Cluster 전역 자원 할당
    - Node Manager : 각 Node의 작업 실행 및 자원 모니터링
3. Operating Mechanism
    - Resource Manager와 Node Manager의 역할 분할
        - ResourceManager : 자원 할당
        - Node Manager : 실행 및 작업 분배