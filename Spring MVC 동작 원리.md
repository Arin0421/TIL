1. DispatcherServlet이 브라우저로부터 요청을 받는다.
2. DispatcherServlet은 요청된 URL을 HandlerMapping 객체에 넘기고, 호출해야 할 Controller와 Method(Handler) 정보를 얻는다.
3. DispatcherServlet이 HandlerAdapter 객체를 가져온다.
4. HandlerAdapter 객체의 메소드를 실행한다.
5. Controller 객체는 비즈니스 로직을 처리하고, 그 결과를 바탕으로 View에 전달할 객체를 Model 객체에 전달한다. DispatcherServlet에게 view name을 return 한다.
6. DispatcherServlet은 view name을 View Resolver에게 전달하여 view 객체를 얻는다.
7. DispatcherServlet은 view 객체에 화면 표시를 의뢰한다.
8. view 객체는 해당하는 뷰를 호출하며, 뷰는 Model 객체에서 화면 표시에 필요한 객체를 가져와 화면 표시를 처리한다.

[출처]<br>
[Spring MVC 동작원리 / 구성요소](https://starkying.tistory.com/entry/Spring-MVC-%EB%8F%99%EC%9E%91%EC%9B%90%EB%A6%AC-%EA%B5%AC%EC%84%B1%EC%9A%94%EC%86%8C)
