# filter   
### 1. 요약
특정 조건을 만족하는 새로운 배열을 필요로 할 때(조건을 만족하는 값만 **걸러낼** 때) 사용
<br /><br />

### 2. 문법
```javascript
// 화살표 함수
filter((element) => { /* … */ } )
filter((element, index) => { /* … */ } )
filter((element, index, array) => { /* … */ } )

// 콜백 함수
filter(callbackFn)
filter(callbackFn, thisArg)

// 인라인 콜백
filter(function(element) { /* … */ })
filter(function(element, index) { /* … */ })
filter(function(element, index, array){ /* … */ })
filter(function(element, index, array) { /* … */ }, thisArg)
```
<br />

### 3. 인자
- callbackFn: 각 요소에서 실행할 함수. 조건을 만족하면 true, 아니면 false 값을 반환함.
  - element: 배열에서 처리될 현재 요소
  - index: 배열에서 처리될 현재 element의 인덱스
  - array: filter() 의해 호출된 배열
- thisArg: 옵션. callbackFn 실행할 때 this로 사용할 값
<br /><br />

### 4. 설명
주어진 배열의 값들을 오름차순으로 접근해 callbackfn을 통해 true를 반환하는 요소를 기준으로 신규 배열을 만들어 반환함.  
filter 함수는 객체를 직접 사용하거나 변형시키지 않지만 callbackfn을 통해 수정할 수 있음.(문제를 발생시킬 수 있는 원인이 됨)  
callbackfn이 호출되는 범위는 callbackfn이 처음 호출되기 이전이며, map이 순회하는 도중에 추가된 요소는 접근하지 않음.  
반대로 순회하는 도중 수정이 일어나면 변경된 값이 callbackfn에 전달되고 삭제된 요소는 접근하지 않음.
<br /><br />

### 5. 예제
```javascript
const words = ['spray', 'limit', 'elite', 'exuberant', 'destruction', 'present'];

const result = words.filter(word => word.length > 6);

console.log(result);
// expected output: Array ["exuberant", "destruction", "present"]

```
