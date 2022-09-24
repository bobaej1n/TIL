# Number
### 1. 요약
 ES6에 추가된 새로운 컬렉션 전용 반복 구문
<br /><br />

### 2. 문법
```javascript
for (variable of iterable)
  statement
```
<br />

### 3. 설명
for of 구문을 사용하기 위해선 컬렉션 객체가 [Symbol.iterator] 속성을 가지고 있어야 함(직접 명시 가능).
<br /><br />

### 4. 예제
```javascript
const array1 = ['a', 'b', 'c'];

for (const element of array1) {
  console.log(element);
}

// expected output: "a"
// expected output: "b"
// expected output: "c"
```
