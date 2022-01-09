# 10. Collection API 활용



### 1. Collection 개요

- Collection Framework : 배열의 단점을 보완
- List, Set, Map 계열이 존재



### 2. List 계열

- ArrayList
- 초기값은 10개이지만 더 삽입이 되면 바뀜
- 생성자 : 클래스 <데이터 타입> 변수 = new 클래스 <데이터 타입> ();
- iterator : 커서라는 개념을 가지고 모든 데이터를 엑세스 함
- vector : ArrayList와 비슷하지만 동기화 처리가 가능
- enumeration : vectort 의 literator
- LinkedList
- header와 data, tail을 이용함



### 3. Map 계열

- Value, Key를 사용
- HashMap<String, String> users = new HashMap<String, String>();
- 앞이 key, 뒤가 value
- Hashtable : HashMap과 동일함
- 차이점 : null 키와 null 값을 저장 할 수 없음
- 동기화 처리 가능



### 4. Set 계열

- HashSet 
- List와 Set의 차이점 : 저장되는 순서가 의미없음, 중복된 값을 저장할 수 없음

