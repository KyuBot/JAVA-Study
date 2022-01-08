# 9. API



### 1. API 문서

- 라이브러리 : 다양한 기능을 가진 코드들의 집합
- 자바 API : 클래스 파일 형태로 제공하는 라이브러리
  - java.io : 외부 데이터 입력 또는 출력을 처리
  - java.lang : 프로그램 개발 시 기본적으로 필요한 기능 ( 유일하게 import 선언 없이 쓸 수 있는 기능)
  - java.sql : 데이터베이스 처리에 관한 기능
  - java.util : 날짜, 시간, 콜렉션 처리에 관한 기능



### 2. 기본 API

- object 
  - hashCode() : 사람의 주민번호처럼 인스턴스의 고유번호를 생성하는 메소드
  - getClass()
    - 메소드 선언부 : public final Class <?> getClass()
    - Class 타입의 객체를 생성하여 리턴함
    - Class 객체는 클래스에 대한 정보를 가지는 객체임
  - toString()
    - 메소드 선언부 : getClass().getName() + '@' + Integer.toHexString(hashCode())
    - 인스턴스에 대한 정보를 문자열로 리턴함
  - equals()
    - 메소드 선언부 : public boolean equals(Object Obj)
- String 
  - 문자열 처리에 관한 기능을 제공하는 객체
  - 원본 변경 불가
- StringBuffer/StringBuilder
  - 문자열 처리에 관한 기능을 제공하는 객체
  - 원본 변경 가능
    - StringBuffer: 동시 접근 기능 처리
    - StringBuilder : 동시 접근 기능 처리 안 함
- Math : 수학적인 계산처리에 관한 기능을 제공하는 객체
- Wrapper 클래스
  - 기본 데이터 타입과 맵핑되는 클래스
  - Boxing/Unboxing : 기본타입 -> 클래스 타입 , 클래스타입 (boxing) -> 기본타입 (unboxing)
  - autoboxing : boxing과 unboxing 작업을 자동으로 처리하는 기능



### 3. 유틸 API

- StringTokenizer
  - 문자열을 분리하는 기능을 가진 객체
- Random
  - 난수를 발생하는 기능을 가진 객체
- Arrays 
  - 배열에 관련된 기능을 제공하는 객체
- Date/Calendar
  - 날짜와 시간에 관련된 기능을 처리하는 객체들
- SimpleDateFormat
  - 날짜와 시간의 포맷 지정을 처리하는 객체
    - y: 연도, M: 월, d: 일 , D: 1~365, E :월화수목금토일
- MessageFormat
  - 문자열의 포맷 지정을 처리하는 객체
- DecimalFormat
  - 숫자의 포맷 지정을 처리하는 객체

