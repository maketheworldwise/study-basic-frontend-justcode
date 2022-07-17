## 🔖 Week-03 Study Keywords

### 1. About variable

- 가독성 및 유지보수 향상
- 중복 제거

```javascript
var num = 0;
let str = "String";
const isTrue = true;
```

### 2. Javascript Data Type

> 참고: https://developer.mozilla.org/ko/docs/Web/JavaScript/Data_structures

- `typeof` 키워드로 타입 확인
- Boolean 타입
- Null 타입
- Undefined 타입
- Number 타입
- BigInt 타입
- String 타입
- Symbol 타입

### 3. `number` & `string` Method

- `Number.isNaN()` : is Not A Number 유효성 검사
- `Number.toString()` : Number -> String 타입 변환
- `Number.isInteger()` : 정수인지 유효성 검사
- `String.indexOf()` : 특정 문자와 일치하는 인덱스 번호 반환
- `String.toLowerCase()` : 문자열을 모두 소문자로 변경
- `String.toUpperCase()` : 문자열을 모두 대문자로 변경
- `String.slice()` : 특정 인덱스 범위를 자르고 반환

### 4. About Function

- 함수는 특정 기능을 수행하도록 설계된 독립적인 코드 블록
- 재사용성, 가독성, 모듈화

```javascript
function addFunc1(num1, num2) {
  return num1 + num2;
}

const addFunc2 = function (num1, num2) {
  return num1 + num2;
};

const addFunc3 = (num1, num2) => {
  return num1 + num2;
};

const addFunc4 = (num1, num2) => num1 + num2;
```

### 5. About Conditional Statement

- "만약 ~ 라면"
- 특정 상황이나 조건에 따른 결정을 만들기 위해 현실의 상황을 모델링

### 6. About Array

- 관련있는 데이터를 하나의 변수에 할당하여 관리하기 위해 사용
- 가독성 증가

```javascript
let arr = [1, 2, 3, 4, 5];
console.log(arr[0]);

// 추가
arr.push(6);
arr.unshift(0);

// 수정
arr[0] = -1;

// 삭제
arr.pop();
arr.shift();
```
