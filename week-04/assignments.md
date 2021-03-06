## π Week-04 Study Keywords

### 1. About Loop

- λ°λ³΅μ μΈ κ³μ°μ μννκΈ° μν΄ μ¬μ©

```javascript
for (let i = 0; i < 10; i++) {
  console.log(i);
}
```

### 2. About Array Loop

- μμ°¨μ μΌλ‘ ν λΉλ λ°°μ΄μ λ°μ΄ν°λ₯Ό λ°λ³΅μ μΌλ‘ λ€λ£° λ μ μ©

```javascript
for (let idx in arr) {
  console.log(arr[i]);
}
```

### 3. About Array Method

> μ°Έκ³  : https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/Array

- `Array.indexOf` : λ°°μ΄μμ μνλ λ°μ΄ν°λ₯Ό μ°Ύκ³ μν  λ μ¬μ©
- `Array.filter()` : λ°°μ΄μμ μ‘°κ±΄μ ν΄λΉνλ λ°μ΄ν°λ₯Ό μ°Ύκ³ μν  λ μ¬μ©
- `Array.forEach()` : forλ¬Έκ³Ό λμΌνκ² λμμ μν
- `Array.map()` : λ°°μ΄ λ΄μ λͺ¨λ  μμ κ°κ°μ λνμ¬ μ£Όμ΄μ§ ν¨μλ₯Ό νΈμΆν κ²°κ³Όλ₯Ό λͺ¨μ μλ‘μ΄ λ°°μ΄λ‘ λ°ν
- `Array.slice()` : λ°°μ΄ λ΄μ νΉμ ν μμμ μΈλ±μ€ λ²μμ λ°λΌ μλ‘μ΄ λ°°μ΄μ λ°ν
- `Array.splice()` : λ°°μ΄ λ΄μ νΉμ ν μμλ₯Ό μ­μ νκ±°λ λμ²΄ν  λ μ¬μ©
- `Array.concat()` : μ£Όμ΄μ§ λ°°μ΄μ κΈ°μ‘΄ λ°°μ΄μ ν©μ³ μλ‘μ΄ λ°°μ΄λ‘ λ°ν
- `Array.sort(), Array.reverse()` : λ°°μ΄μ λ°μ΄ν°λ₯Ό μ λ ¬νκ±°λ μμλ₯Ό λ€μ§κ³ μν  λ μ¬μ©

### 4. About Object

- κ°μ²΄λ μ°Έμ‘°ν λ°μ΄ν°μ ν μ€ νλλ‘ μ¬λ¬κ°μ λ°μ΄ν°λ₯Ό λ΄μ λ μ¬μ©
- κ΄λ ¨μλ λ°μ΄ν°λ₯Ό λ¬Άμ΄μ μ²λ¦¬ν  μ μκΈ° λλ¬Έμ μ½λμ μ μ§λ³΄μμ± μ¦κ°
- μ€μΈκ³μ μ¬κ³ λ°©μκ³Ό μ μ¬νλλ‘ μ€κ³ κ°λ₯
- λ°°μ΄μ μμ μλ£νμ΄ μλ κ°μ²΄νμ μνκΈ° λλ¬Έμ κ°μ²΄μ²λΌ λμ (λ°°μ΄μ μμκ° λ³΄μ₯λλ κ°μ²΄λ‘ λ³΄λ νΈμ΄ μ¬μ)
- `Object.keys(obj)` : κ°μ²΄μ ν€λ§ λ΄μ λ°°μ΄μ λ°ν
- `Object.values(obj)` : κ°μ²΄μ κ°λ§ λ΄μ λ°°μ΄μ λ°ν
- `Object.entries(obj)` : [ν€, κ°] μμ λ΄μ λ°°μ΄μ λ°ν

```javascript
let obj = {
  "hello world": "test",
  key1: "value1",
  key2: "value2",
};

console.log(obj.key1);
console.log(obj["hello world"]);

// μΆκ°
obj.key3 = "value3";
obj[key4] = "value4";

// μμ 
obj.key3 = "value3 update";
obj[key4] = "value4 update";

// μ­μ 
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
