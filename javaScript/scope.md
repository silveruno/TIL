# 11. 유효범위 (Scope)

- javaScript : 함수레벨 스코프를 가진다.
  - 함수의 코드블록안만 지역이고, 나머지는 모두 전역 취급
- 기타언어 : 블록레벨 스코프를 가진다.

- 암묵적 전역 : 함수 내부에 선언되지 않은 변수의 값을 재할당하면, 자바스크립트 엔진은 해당 변수명을 찾기 못하기에 전역에 선언한 것으로 동작한다.

- 렉시컬 스쿠핑 : 선언된 시점의 환경에서 스쿠핑하는 것. 지역 안에 다른 함수를 호출해서 사용한다 하더라도 선언된 시점에 지역 밖에 있었던 것으로 인식.

- 전역변수의 무분별한 사용은 무척 위험하다. 스코프는 좁을 수록 좋다.
  - IIFE를 활용, 클래스로 작성, ES6모듈 활용 등의 방법