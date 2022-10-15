#    
### 1. 요약
유사 배열 객체(array-like object)나 반복 가능한 객체(iterable object)를 얕게 복사해 새로운 Array 객체를 만듦.
<br /><br />

### 2. 문법
```javascript
// Arrow function
Array.from(arrayLike, (element) => { /* … */ } )
Array.from(arrayLike, (element, index) => { /* … */ } )

// Mapping function
Array.from(arrayLike, mapFn)
Array.from(arrayLike, mapFn, thisArg)

// Inline mapping function
Array.from(arrayLike, function mapFn(element) { /* … */ })
Array.from(arrayLike, function mapFn(element, index) { /* … */ })
Array.from(arrayLike, function mapFn(element) { /* … */ }, thisArg)
Array.from(arrayLike, function mapFn(element, index) { /* … */ }, thisArg)
```
<br />

### 3. 인자
- arrayLike: 배열로 변환할 수 있는 반복할 수 있거나 배열 같은 객체
- mapFn: 배열의 모든 요소를 호출하는 기능을 하는 map
- thisArg: mapFn을 실행할때 this로 사용되는 값
<br /><br />

### 4. 반환값
새로운 Array 인스턴스
<br /><br />

### 5. 예제
```javascript
console.log(Array.from('foo'));
// expected output: Array ["f", "o", "o"]

console.log(Array.from([1, 2, 3], x => x + x));
// expected output: Array [2, 4, 6]
```
