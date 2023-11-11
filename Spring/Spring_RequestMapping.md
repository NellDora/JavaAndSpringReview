# RequestMapping

[RequestMapping]    <br>
URL이 호출되면 호출되는 애노테이션이다.     <br>

메소드 앞에 작성하여 사용한다.                                           <br>
(Ex)                                                                     <br> 
@RequestMapping(value = "URL 주소" , Method= "GET" or "POST")       <br>
public ModelAndView [메서드명]                                       <br>
ModelAndView mav = new ModelAndView ("템플릿 주소");                 <br>
mav.addObject("testUser", testUser);                                <br>
retureturn mav;                                                     <br>
<br><br>
Method를 통해 Get방식의 형식 혹은 Post방식의 형식을 선택하여 사용할 수 있다.      <br>
그럼 위의 ModelAndView는 무엇인가?                                       <br>
ModelAndView는 데이터, 뷰를 관리하는 클래스이다        <br>
Model : 화면상에서 사용하는 객체 데이터등등을 전달한다       <br>
View : 화면에 보이는 뷰를 호출할때 사용되며 템플릿의 경로를 이용한다<br>

<hr>

RequestMapping을 이용하여 URL 매핑을 할수도 있지만 다른 방법 또한 존재한다.     <br>
                                                                        <br>
(1) GetMapping                                                          <br>
RequestMapping의 Get 형식의 버전이며 기능도 동일하다   <br>
@GetMapping("/URL주소")                                               <br>
public String getExam(){                                              <br>
return "템플릿 주소";                                                    <br>
}                                                                      <br>

<br><br>
(2) PostMapping                                                          <br>
RequestMapping의 Post 형식의 버전이며 기능도 동일하다   <br>
@GetMapping("/URL주소")                                               <br>
public String postExam(){                                              <br>
return "템플릿 주소";                                                    <br>
}                                                                      <br>


