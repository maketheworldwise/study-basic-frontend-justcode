## π Week-03 Study Keywords

### 1. About variable

- κ°λμ± λ° μ μ§λ³΄μ ν₯μ
- μ€λ³΅ μ κ±°

```javascript
var num = 0;
let str = "String";
const isTrue = true;
```

### 2. Javascript Data Type

> μ°Έκ³ : https://developer.mozilla.org/ko/docs/Web/JavaScript/Data_structures

- `typeof` ν€μλλ‘ νμ νμΈ
- Boolean νμ
- Null νμ
- Undefined νμ
- Number νμ
- BigInt νμ
- String νμ
- Symbol νμ

### 3. `number` & `string` Method

- `Number.isNaN()` : is Not A Number μ ν¨μ± κ²μ¬
- `Number.toString()` : Number -> String νμ λ³ν
- `Number.isInteger()` : μ μμΈμ§ μ ν¨μ± κ²μ¬
- `String.indexOf()` : νΉμ  λ¬Έμμ μΌμΉνλ μΈλ±μ€ λ²νΈ λ°ν
- `String.toLowerCase()` : λ¬Έμμ΄μ λͺ¨λ μλ¬Έμλ‘ λ³κ²½
- `String.toUpperCase()` : λ¬Έμμ΄μ λͺ¨λ λλ¬Έμλ‘ λ³κ²½
- `String.slice()` : νΉμ  μΈλ±μ€ λ²μλ₯Ό μλ₯΄κ³  λ°ν

### 4. About Function

- ν¨μλ νΉμ  κΈ°λ₯μ μννλλ‘ μ€κ³λ λλ¦½μ μΈ μ½λ λΈλ‘
- μ¬μ¬μ©μ±, κ°λμ±, λͺ¨λν

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

- "λ§μ½ ~ λΌλ©΄"
- νΉμ  μν©μ΄λ μ‘°κ±΄μ λ°λ₯Έ κ²°μ μ λ§λ€κΈ° μν΄ νμ€μ μν©μ λͺ¨λΈλ§

### 6. About Array

- κ΄λ ¨μλ λ°μ΄ν°λ₯Ό νλμ λ³μμ ν λΉνμ¬ κ΄λ¦¬νκΈ° μν΄ μ¬μ©
- κ°λμ± μ¦κ°

```javascript
let arr = [1, 2, 3, 4, 5];
console.log(arr[0]);

// μΆκ°
arr.push(6);
arr.unshift(0);

// μμ 
arr[0] = -1;

// μ­μ 
arr.pop();
arr.shift();
```
