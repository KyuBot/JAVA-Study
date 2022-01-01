# 1. 자바의 소개

### 1. 프로그램 언어
> 처리를 목적으로 존재하는것 

### 2. 자바의 역사
- 세계에서 가장 많이 쓰이는 언어
- 소스파일 (컴파일) -> 실행파일 (실행) -> 컴퓨터

### 3. 프로그램 개발 순서
> System.out.print("직진하시오");

  1. 소스파일 (자연어): 인간중심으로 표현된 언어
  2. 실행파일 (기계어): 1과 0으로 작성된 명령문
  3. 컴파일 : 소스파일을 기계어로 변환
     1. java -> class
  4. java -> class (바이트코드) -> JVM (기계어코드) -> 컴퓨터

### 4. JVM (Java Virtual Machine)
> class loader -> byte code verifier -> interpreter & just-in-time compiler -> runtime system 

1. class loader : 프로그램을 실행하기 위해 필요한 파일들을 찾아 컴퓨터에 사용할 수 있도록 준비작업을 해주는 기능 (필요한 것들을 모두 메모리에 로딩)
2. byte code verifier : 준비된 코드들의 유효성 검증
3. interpreter/JIT compiler : byte 코드를 기계어로 변환
4. interpreter : 명령문 단위로 기계어 변환
5. JIT compiler : 전체를 한번에 기계어로 변환

### 5. JDK
> JDK : JVM + 개발 Tool (개발까지 하려면)

> JRE : JVM + api (단순히 실행)

> JAVA_HOME : Java 환경변수

> path 환경변수 : 실행 위치에 프로그램이 존재하지 않아도 실행할 수 있도록 함. JAVA_HOME/bin 폴더를 path에 추가함 (%JAVA_HOME%\bin)

> 컴파일러 : javac (소스코드 -> 바이트 코드) / 실행도구 : java.exe 자바 실행프로그램 / 압축 도구 : jar (자바 언어에서 사용하는 표현 압축 파일 형식) / 문서작성도구 : javadoc (작성된 파일에 대한 정보문서를 만드는 도구)

### 6. 이클립스

- 이클립스는 프로젝트 단위로 생성
- new -> project -> java project -> JRE

### 7. 실행
> 컴파일 : javac 파일명.java

> 실행 : java 파일명 (이때 .class는 쓰지않는다)
