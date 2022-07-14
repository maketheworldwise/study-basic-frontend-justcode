## Javascript Event

- 사용자의 이벤트의 종류와 감지
- Key Event로 용사 움직이기

---

## DOM Event

- https://www.w3schools.com/jsref/dom_obj_event.asp

## Key Event

- js 선언 스크립트들은 모두 하나의 문서로 취급
- js 선언 순서가 중요
- 강의에서는 settings.js에 요소의 변수를 모두 선언하여 사용
- 브라우저에서는 이벤트 정보를 넘기도록 파라미터 지정
- 픽셀 단위를 사용할 때, 증감은 단위 문자열을 제거해주고 숫자로 형변환을 해서 처리

## onClick vs addEventListener

> 참고: https://jiwondev.tistory.com/28

onClick 속성을 이용한 방법은 웹 초창기에 사용한 방법이라 올드하고 한가지 이벤트만을 가지게 된다면, addEventListner의 경우 onClick에 비해 조금 더 최신 기술이며, 모든 이벤트가 객체로 관리되고 여러개를 등록 할 수 있다는 점에서 onClick을 지양하는 편.

## console.log 성능

- 보안적인 요소
- https://velog.io/@kimbiyam/Javascript-console.log-%EC%86%8D%EB%8F%84-%EA%B4%80%EB%A0%A8

## input과 label을 사용하는 이유

- 웹 접근성을 위해 (시각 장애인)
