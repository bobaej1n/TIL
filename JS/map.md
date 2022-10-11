# map   
### 1. 요약
배열의 값을 재정의 할 때 사용하는 메서드
<br /><br />

### 2. 문법
```javascript
// 화살표 함수
map((element) => { /* … */ })
map((element, index) => { /* … */ })
map((element, index, array) => { /* … */ })

// 콜백 함수
map(callbackFn)
map(callbackFn, thisArg)

// 인라인 콜백 함수
map(function(element) { /* … */ })
map(function(element, index) { /* … */ })
map(function(element, index, array){ /* … */ })
map(function(element, index, array) { /* … */ }, thisArg)
```
<br />

### 3. 인자
- callbackFn: 각 요소에서 실행할 함수
  - element: 배열에서 처리될 현재 요소
  - index: 배열에서 처리될 현재 element의 인덱스
  - array: map에 의해 호출된 배열
- thisArg: 옵션. callbackFn 실행할 때 this로 사용할 값
<br /><br />

### 4. 설명
주어진 배열의 값들을 오름차순으로 접근함.  
이때 callbackfn을 통해 새로운 값을 정의하고 신규 배열을 만들어 반환함.  
map 함수는 객체를 직접 사용하거나 변형시키지 않지만 callbackfn을 통해 수정할 수 있음.(문제를 발생시킬 수 있는 원인이 됨)  
callbackfn이 호출되는 범위는 callbackfn이 처음 호출되기 이전이며, map이 순회하는 도중에 추가된 요소는 접근하지 않음.  
반대로 순회하는 도중 수정이 일어나면 변경된 값이 callbackfn에 전달되고 삭제된 요소는 접근하지 않음.
<br /><br />

### 5. 예제
```javascript
const numbers = [1, 2, 3, 4, 5];
const result = numbers.map(number => number * number);

console.log(numbers);
// [1, 2, 3, 4, 5];

console.log(result);
// [1, 4, 9, 16, 25]
```
