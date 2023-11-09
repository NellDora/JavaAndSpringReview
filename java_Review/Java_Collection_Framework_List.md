# Collection Framework (컬렉션 프레임 워크)

<h3> List를 알아봅시다 </h3>

[List]<br>
저장 데이터의 순서 유지 O, 중복 허용 O  <br>
저장되는 데이터는 저장 시점에서 자동으로 인덱스가 부여됨

구현 클래스 ArrayList, Vector, LinkedList 등 <br>
<hr>
[List 메서드]  <br>
(1) add 값을 추가 <br>
list.add(1);        <br>

<br>

(2) Object get(int index) : index에 해당하는 요소 리턴 <br>
System.out.println("2번째에 저장된 값 : " + list.get(2));  <br>
<br>
(3) int indexOf(Object o) : 특정 요소가 위치한 인덱스 리턴 (앞에서부터 탐색)  <br>
System.out.print("정수 3의 인덱스 : " + list.indexOf(3));             <br>
<br>
(4) Object remove(int index) : index에 해당하는 요소 삭제 후 요소 리턴    <br>
요소가 정수 타입일 경우 정수 데이터를 지정하면 정수 데이터가 아닌 인덱스 취급   <br>
<br>
(5) add (int index, Object o ) : 특정 인덱스에 해당 요소(O)를 추가       <br>
list.add(1,5); -> 1번 인덱스에 5추가               <br>
<br>
(6) set(int index, Object o) : 특정 인덱스에 해당 요소(o)를 덮어씀        <br>
list.set(1, 10); -> 1번 인덱스에 10 추가 (기존 데이터 덮어쓰기)             <br>
<br>
(7) List subList(int beginIndex, int endIndex)                      <br>
List subList = list.subList(1,3);   -> 1 ~ 3까지 추출 (1 ~ 2)       <br>
<br>

<hr>
[Collections 클래스]
<br>
(1) Collections.sort(List) : List 객체 정렬 ( 같은 타입 요소만 가능)     <br>
Collections.sort(list2);                                            <br>
<br>
(2) Collections.shuffle(list2);
Collections.shuffle(list2) -> List 객체 무작위 섞기 (타입 상관 X)
