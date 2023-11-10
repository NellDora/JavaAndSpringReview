# Collection Framework (컬렉션 프레임 워크)

<h3> Map를 알아봅시다 </h3>

[Map]<br> 
Key, Value를 한쌍으로 갖는 자료 구조<br>
-> 키는 중복 X , Value는 중복 O        <br>


구현 클래스 HashSet, Properties 등 <br>
<hr>
[Map 메서드]  <br>
(1) put(Object key, Object value) :  키에 해당하는 데이터 (Value) 추가 <br>
map.put(1,"빠삐꼬")        <br>
map.put(2, "호두마루")      <br>
map.put(3, "생귤탱귤")      <br>
-> 키는 중복이 불가능하며 이미 존재하는 Key에 value를 추가하면 덮어짐<br>
<br>

(2) Object get(Object key) : key에 해당하는 값 리턴 <br>
map.get(2); -> 정수 2에 해당하는 value 리턴      <br>
<br>

(3)Set keySet() : Map 객체 내의 모든 값 리턴     <br>
Set keySet = map.keySet();                  <br>
<br>

(4) Collection values() : Map 객체 내의 모든 값 리턴 <br>
List valueList = new ArrayList(map.values());   <br>
<br>

(5)entrySet() : 키 = 값을 한쌍으로 갖는 엔트리 객체를 Set타입으로 리턴  <br>
Set entrySet = map.entrySet();                              <br>
<br>

containsValue() : 특정 값을 탐색                              <br>
boolean result = map.containValue("PPAP");                  <br>
<br>

containKey() : 특정 키 탐색                                  <br>
boolean result = map.containValue(4);

