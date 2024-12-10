# Atomicity
Transaction의 모든 Operation들이 Database에 반영되거나 혹은 아무것도 반영되면 안됨

# Consistency
Transaction의 Execution의 isolation은 Database의 Consistency를 확보해야 함

# Isolation
여러 Transaction이 Concurrently하게 Execution 되어도, 각각의 Transaction은 서로 간섭할 수 없음

# Durability
성공적으로 완료된 Transaction의 변경사항은 System Failure에도 유지되어야 함