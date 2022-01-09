# 11. 예외처리



### 1. 자바 예외 API

- 예외 처리 객체 구조



### 2. 예외 처리 방법

- try - catch 문

  ```java
  try{
      일반 실행문
  }catch(변수선언){
      오류 처리 실행문
  }finally{
      항상 수행할 실행문
  }
  ```

- 전체 예외를 처리하고 싶으면 catch(Exception e)

- 에러 메세지 출력 e.getMessage();

- 역추적 : e.printStackTrace();

- finally : try 블록의 오류 발생 여부와 상관없이 try 블록을 빠져나올때 항상 실행 됌

- 주로 자원 해제 할때 씀

- try-with-resources : java 7 이상에서 사용 가능

  - 자원 해제를 쉽게 하기 위해서 사용
  - finally{ fi.close(); fo.close(); } 이렇게 사용해야 할 것을
  - try( 이곳에서 자원해제를 시켜 놓음 ) 



### 3. throws 선언문

- throws 필요성
  - 메소드 선언부에 사용함
  - throws 다음에 콤마(,) 를 구분자로 처리할 Exception 이름을 나열함



### 4. 사용자 정의 예외 객체

- 객체 선언
  - Exception을 상속받음
  - 객체의 이름에 ~Exception을 사용함
- throw : 오류를 강제로 발생시키는 명령문

