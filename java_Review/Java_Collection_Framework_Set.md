# Collection Framework (컬렉션 프레임 워크)
<h2>컬렉션 프레임 워크란?</h2>
컴퓨터 시스템에서 데이터를 효율적으로 저장 및 관리하는 것 (흔히 말하는 자료 구조)

<hr>

인터페이스 종류 <br>
1.Set : 저장를 유지하지 않는다, 값 중복 허용          <br>
2.List : 저장 데아터의 순서를 유지, 값의 중복을 허용          <br>
3.Map : 키(Key)와 값(Value)이 한쌍인 자료 구조 , 키 (중복 불허용), 값(중복 허용)

<br>
<hr>
----------------------------상세하게 알아보기------------------<br>
<h3>Set을 알아봅시다</h3>
구현체 클래스 : HashSet, TreeSet 등등 <br>
선언 방식 : 1. HashSet set = new HashSet(); / 2. Set set = new HashSet();         <br>

[Set의 메서드] <br>
(1) boolean isEmpty() : 컬렉션 객체가 비어있는지 여부 리턴     <br>
boolean test = set.isEmpty();                           <br><br>

(2) int size() : 컬렉션 객체에 저장된 요소 (데이터, 객체) 개수 리턴 <br>
int totalCount = set.size();                            <br><br>

(3) boolean add(Object o) : 컬렉션 객체에 요소(o (데이터))를 추가 <br>
set.add(5); &nbsp; / set.add(user3);                        <br>
저장이 성공하면 true 반환, 이미 값이 존재하여 중복이 되어서 저장이 불가능 하면 false 반환 <br><br>

(4) boolean contain(Object o) : 컬렉션 객체 요소에 (o)가 있는지 결과값 리턴 <br>
System.out.print("set에 2000 값이 있나요? : " + set.contain(2000)); <br><br>

(5) booeal remove(Object o ): 컬렉션 객체 내의 요소 o를 삭제 (성공 여부 리턴) <br>
System.out.println("findUser 삭제가 성공 했는가? : " + set.remove(finduser));   <br><br>

(6) void clear() :  컬렉션 요소 초기화 <br>
set.clear();                    <br><br>

Object[] toArray() : 컬렉션을 배열로 변환    <br>
Object[] oArr = set.toArray();      <br><br>

<hr>
TreeSet : 같은 타입 데이터가 저장된 Set 객체 정렬 가능 <br>
-> 단, 같은 데이터만 정렬 가능  <br>
-> 수치 데이터는 숫자 크기 순으로 오름차순 정렬 <br>

<hr>
Iterator(반복자)  <br>
1. 컬렉션 객체 (Set 또는 List)의 iterator() 메서드를 호출, Iterator 인터페이스를 구현한 객체를 리턴 <br>
2. while문을 통해 Iterator 객체의 hasNext() 메서드가 true일때 동안 반복
3. 반복문 내에서 Iterator 객체의 next() 메서드를 통해 데이터 가져옴

