# **재고시스템으로 알아보는 동시성이슈 해결방법**

**RaceCondition이란?**

Race Condition은 둘 이상의 프로세스 또는 스레드가 공유 자원에 접근하려고 할 때 발생할 수 있는 문제입니다. 이 문제는 동시성 제어에 대한 실수 또는 버그로 인해 발생할 수 있습니다.

**해결방법**

- 첫 번째는 락(lock)을 사용하는 것입니다.
    - 락은 공유 자원에 대한 접근을 제어하여 동시에 여러 스레드 또는 프로세스가 동시에 접근하지 못하도록 합니다.
- 두 번째로는 트랜잭션(transaction)을 사용하는 것입니다.
    - 트랜잭션은 데이터베이스 등에서 여러 개의 작업을 하나의 단위로 묶어서 실행하는 것으로, 이를 통해 데이터의 일관성을 유지할 수 있습니다.
