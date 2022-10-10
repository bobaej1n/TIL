# forEach
### 1. 요약
**배열에서만** 사용하는 배열 반복문 메서드
<br /><br />

### 2. 문법
```javascript
// 화살표 함수
forEach((element) => { /* … */ })
forEach((element, index) => { /* … */ })
forEach((element, index, array) => { /* … */ })

// 콜백 함수
forEach(callbackFn)
forEach(callbackFn, thisArg)

// 인라인 콜백 함수
forEach(function(element) { /* … */ })
forEach(function(element, index) { /* … */ })
forEach(function(element, index, array){ /* … */ })
forEach(function(element, index, array) { /* … */ }, thisArg)
```
<br />

### 3. 인자
- callbackFn: 각 요소에서 실행할 함수
  - element: 배열에서 처리될 현재 요소
  - index: element 배열의 인덱스
  - array: forEach()에 의해 호출된 배열
- thisArg: 옵션. callbackFn 실행할 때 this로 사용할 값
<br /><br />

### 4. 설명
배열의 처음부터 마지막 요소까지 반복하여 실행함.  
인자로 콜백 함수를 받아옴.  
주어진 콜백 함수를 배열 요소 각각에 대해 실행함.
<br /><br />

### 5. 예제
```javascript
const array1 = ['a', 'b', 'c'];

array1.forEach(element => console.log(element));

// expected output: "a"
// expected output: "b"
// expected output: "c"
```
