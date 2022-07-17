## 🔖 Week-04 Study Keywords

### 1. About Loop

- 반복적인 계산을 수행하기 위해 사용

```javascript
for (let i = 0; i < 10; i++) {
  console.log(i);
}
```

### 2. About Array Loop

- 순차적으로 할당된 배열의 데이터를 반복적으로 다룰 때 유용

```javascript
for (let idx in arr) {
  console.log(arr[i]);
}
```

### 3. About Array Method

> 참고 : https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Array

- `Array.indexOf` : 배열에서 원하는 데이터를 찾고자할 때 사용
- `Array.filter()` : 배열에서 조건에 해당하는 데이터를 찾고자할 때 사용
- `Array.forEach()` : for문과 동일하게 동작을 수행
- `Array.map()` : 배열 내의 모든 요소 각각에 대하여 주어진 함수를 호출한 결과를 모아 새로운 배열로 반환
- `Array.slice()` : 배열 내의 특정한 요소의 인덱스 범위에 따라 새로운 배열을 반환
- `Array.splice()` : 배열 내의 특정한 요소를 삭제하거나 대체할 때 사용
- `Array.concat()` : 주어진 배열에 기존 배열을 합쳐 새로운 배열로 반환
- `Array.sort(), Array.reverse()` : 배열의 데이터를 정렬하거나 순서를 뒤집고자할 때 사용

### 4. About Object

- 객체는 참조형 데이터유형 중 하나로 여러개의 데이터를 담을 때 사용
- 관련있는 데이터를 묶어서 처리할 수 있기 때문에 코드의 유지보수성 증가
- 실세계의 사고방식과 유사하도록 설계 가능
- 배열은 원시 자료형이 아닌 객체형에 속하기 때문에 객체처럼 동작 (배열은 순서가 보장되는 객체로 보는 편이 쉬움)
- `Object.keys(obj)` : 객체의 키만 담은 배열을 반환
- `Object.values(obj)` : 객체의 값만 담은 배열을 반환
- `Object.entries(obj)` : [키, 값] 쌍을 담은 배열을 반환

```javascript
let obj = {
  "hello world": "test",
  key1: "value1",
  key2: "value2",
};

console.log(obj.key1);
console.log(obj["hello world"]);

// 추가
obj.key3 = "value3";
obj[key4] = "value4";

// 수정
obj.key3 = "value3 update";
obj[key4] = "value4 update";

// 삭제
delete obj.key3;
delete obj.key4;
```

```javascript
let obj = {
  read : [
    arr1 : [
      idx1 : {
        "id": 1
      },
      idx2 : {
        "id": 2
      }
    ],
    arr2 : [
      idx3 : {
        "id": 3
      },
      idx4 : {
        "id": 4
      }
    ]
  ]
}

console.log(obj.read[0].arr1[0].idx1["id"]);
```

```javascript
let obj = {
  key1: "value1",
  key2: "value2",
};

for (let key in obj) {
  console.log("key : ", key);
  console.log("key : ", obj[key]);
}
```
