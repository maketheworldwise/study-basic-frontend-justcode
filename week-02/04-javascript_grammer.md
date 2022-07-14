## Javascript Grammer

- if문, 비교/논리 연산자
- 배열과 반복문
- 함수 - 선언과 호출
- 함수 - 값 변환하기
- 함수 - 데이터 받아서 활용, 매개변수와 인자
- 주기적으로 코드 실행 (1)
- 주기적으로 코드 실행 (2)

---

## 가변인자를 가지는 함수

```javascript
function meetAt(...args) {
  if (args.length === 1) {
    return args[0] + "년";
  } else if (args.length === 2) {
    return args[0] + "년" + " " + args[1] + "월";
  } else if (args.length === 3) {
    return args[0] + "/" + args[1] + "/" + args[2];
  } else {
    return -1;
  }
}
```
