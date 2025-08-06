.
* loginSuccessHandler - AuthenticationSuccessHandler를 반환하는 Bean 메소드

* AuthenticationSuccessHandler 인터페이스는 는 로그인 성공시에 행할 동작을 정의하는 인터페이스

  * SavedRequestAwareAuthenticationSuccessHandler 는AuthenticationSuccessHandler 를 구현함
  -SavedRequestAwareAuthenticationSuccessHandler 란?
  로그인전에 사용자가 접근하려던  url을 기억하고 있다가 로그인 후 기억했었던 url로 자동 redirect해주는 기능이 있음


* 이 빈에서는 onAuthenticationSuccess 를 오버라이드 중
  - 세션에 redirectAfterLogin 속성이 있으면 그 url로 이동하고
  - 없으면 기본 savedRequestAwareAutenticationSuccessHandler의 로직을 따름
