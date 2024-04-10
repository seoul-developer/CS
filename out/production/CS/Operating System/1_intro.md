## 💋 What is OS?

### ✔️ 정의

- 하드웨어 자원을 애플리케이션에서 사용할 수 있도록 하는 소프트웨어
- Software that converts hardware into a useful form for applications

## ✔️ 기능

- 소프트웨어 관점에서
    - 프로그램의 실행 환경 제공
    - 하드웨어 자원을 _추상화된 형태로_ 제공
- 시스템의 관점에서
    - 컴퓨터 시스템의 자원(CPU, Memory, I/O devices 등등)을 관리
- 구현 관점에서
    - event driven
        - 애플리케이션은 system call과 같은 trap으로 OS를 호출
        - 하드웨어는 interrupt로 OS를 호출

## ✔️ 역할

- 하드웨어 자원을 **추상화**
    - 내부 구현은 숨기고, 애플리케이션이 사용할 수 있도록 API 제공
- 격리를 통한 보안
    - 개별 애플리케이션이 요상한 짓을 해서 하드웨어 자원을 망가뜨리는 것을 방지
    - 애플리케이션끼리 격리
- 하드웨어 자원 공유

## ✔️ 공부해야 할 3가지 큰 줄기

- 추상화 (Virtualization)
    - 각 애플리케이션은 현재 컴퓨터 자원을 '나만' 쓰고 있다고 생각하도록 해야 한다.
    - 관련 키워드: Process, CPU Scheduling, Virtual Memory
- 동시성 (Concurrency)
    - 동시다발적으로 일어나는 이벤트들을 정확하게 처리해야 한다.
    - 관련 키워드: synchronization, Thread
- 영속화 (Persistence)
    - 데이터를 영속적으로 안전하게 (컴퓨터 꺼져도 안날라가도록) 저장한다.
    - 관련 키워드: storage, file systems