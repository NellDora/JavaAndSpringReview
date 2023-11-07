# JSON
<h3>JSON (JavaScript Object Notation)이란 Javascript 객체 문법이며 구조화된 데이터를 표현하기 위한 문자 기반의 포맷</h3>

JSON.stringify() <br>
JavaScript에서 JSON.stringify() 함수를 사용하여 객체를 JSON문자열로 사용 가능하다.
<br>
[예]<br>
var user ={"id" : "ppap" , " grade" : "bronze" , " level" : 11  };                  <br>
var stringifyUser - JSON.stringify(user);                                           <br>

<br>
var stringifyUser = '{"id" : "ppap" , " grade" : "bronze" , " level" : 11  }'       <br>
var user - JSON.parse(stringifyUser);                                               <br>

<hr>
JSONObject : JSON 하나에 K/V 쌍으로 들어가 있는 상태 => JSON 데이터에서 {}로 둘러 쌓인 객체   <br>
JSONArray : []로 둘러 쌓인 JSON 배열                                                   <br>
JsonParser : JSON 데이터를 파싱하는 Java 클래스 - JSON을 파싱 , 배열 변환에 사용 가능        <br><br>

parse(String) : JSON -> JsonObject or JsonArray                                     <br>
parse(Reader json) : JSON -> JsonObject or JsonArray                                <br>
parse(InputStream json) : JSON -> JsonObject or JsonArray                           <br>

<hr>
그럼 StringEntity는 무엇일까?



