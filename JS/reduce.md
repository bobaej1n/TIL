# reduce   
### 1. 요약
배열의 각 요소에 대해 주어진 리듀서(reducer) 함수를 실행하고, 하나의 결과값을 반환함.
<br /><br />

### 2. 문법
```javascript
// 화살표 함수
reduce((previousValue, currentValue) => { /* … */ } )
reduce((previousValue, currentValue, currentIndex) => { /* … */ } )
reduce((previousValue, currentValue, currentIndex, array) => { /* … */ } )

reduce((previousValue, currentValue) => { /* … */ } , initialValue)
reduce((previousValue, currentValue, currentIndex) => { /* … */ } , initialValue)
reduce((previousValue, currentValue, currentIndex, array) => { /* … */ }, initialValue)

// 콜백 함수
reduce(callbackFn)
reduce(callbackFn, initialValue)

// 인라인 콜백 함수
reduce(function(previousValue, currentValue) { /* … */ })
reduce(function(previousValue, currentValue, currentIndex) { /* … */ })
reduce(function(previousValue, currentValue, currentIndex, array) { /* … */ })

reduce(function(previousValue, currentValue) { /* … */ }, initialValue)
reduce(function(previousValue, currentValue, currentIndex) { /* … */ }, initialValue)
reduce(function(previousValue, currentValue, currentIndex, array) { /* … */ }, initialValue)

```
<br />

### 3. 인자
- callbackFn: 다음 인자들과 호출되는 reducer 함수
  - previousValue: callbackFn에 대한 이전 호출의 결과 값. 처음 호출 시, initialValue가 명시되어 있지 않으면 array[0]의 값.
  - currentValue: 현재 요소의 값. 처음 호출 시, initialValue가 명시되어 있다면 array[0]의 값이고 그렇지 않으면 array[1]의 값.
  - currentIndex: 배열에서 currentValue의 인덱스 번호. 처음 호출 시, initialValue가 명시되어 있다면 0이고 그렇지 않으면 1.
  - array: 순회 중인 배열
- initialValue: 옵션. 호출될 때 처음에 초기화되는 값.
  - 명시되면 array의 첫번째 값이 currentValue가 됨.
  - 명시되지 않으면 array의 첫번째 값이 previousValue, 두번째 값이 currentValue가 됨.
<br /><br />

### 4. 설명
reduce에는 누산기가 포함되어 있기 때문에, 배열의 각 요소에 대해 함수를 실행하고 누적된 값을 출력할 때 용이함.  
for문이나 count를 위한 별도의 변수를 선언하지 않아도 된다는 장점이 있음.
<br /><br />

### 5. 예제
```javascript
const array1 = [1, 2, 3, 4];

// 0 + 1 + 2 + 3 + 4
const initialValue = 0;
const sumWithInitial = array1.reduce(
  (previousValue, currentValue) => previousValue + currentValue,
  initialValue
);

console.log(sumWithInitial);
// expected output: 10

```
