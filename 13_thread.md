# 13. 스레드



### 1. 스레드

- 하나의 작업의 단위



### 2. 스레드 생성

- class 클래스명 extends Tread {}

- public void run()

- f1.start() 로 run을 시작

- Runnable 인터페이스

  - class 클래스명 implements Runnable {

    }

  - public void run()

  - f1.start() 로 run 을 시작 

- 우선 순위 지정

  - f1.setPriority(Thread.MAX_PRIORITY)
  - f1.setPriority(Thread.MIN_PRIORITY)



### 3. 동기화

- 특정 객체 
  - synchornized (객체) {} => 동기화 처리
  - 동시에 접근 시 한 작업이 끝나기 전에 대기 상태
- 메소드
  - public synchronized void 메소드() {}
- 스레드 상태
  - wait()  : 대기 상태
  - notifyAll() : 작업 끝을 알려줌



### 4. 스레드 제어

- join() : 어떤 스레드의 처리가 종료되었을 때 자신의 스레드를 실행함
- sleep() : 스레드를 지정된 시단동안 일시 정지시킴
- interrupt() : sleep(), wait(), join() 으로 인해 대기중인 스레드의 대기를 취소함
- ThreadPool
  - 실행할 스레드를 미리 생성하여 관리하는 자원
  - 실행 시 pool에서 스레드 대여
  - 실행 종료 후 pool에 반납
- semaphore 
  - java.util.concurrent.Semaphore
  - 실행할 수 있는 스레드 수를 제어하기 위한 카운터 제공