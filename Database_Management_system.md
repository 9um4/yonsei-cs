# 의미
상호 연결된 Data들을 관리하기 위해 사용되는 Program들의 집합

# 목적
- File System을 사용해 Data를 Store하면서 발생하는 문제 해결
    1. Data Redundancy and Inconsistency
    2. Difficulty in Accessing Data
    3. Integrity Problem
    4. Atomicity of Updates
    5. Concurrent Access by Multiple Users
    6. Security Problems

# 구조
1. Application Programs/Queries
    - User, 혹은 Programmer가 Database와 상호작용하기 위해 작성한 Program, 혹은 SQL Query
2. DBMS Software
    - Database의 핵심 역할을 담당하는 Software
    1. Software to Process Queries/Programs
    2. Software to Access Stored Data
3. Stored Database Definition (Meta-Data)
4. Stored Database