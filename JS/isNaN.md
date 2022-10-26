# isNaN (is Not a Number)
### 1. 요약
매개변수가 숫자인지 검사하는 함수
<br /><br />

### 2. 문법
```javascript
isNaN(value)
```
<br />

### 3. 인자
value: 검사할 값
<br /><br />

### 4. 반환값
매개변수가 숫자가 아니면 true, 숫자이면 false를 반환
<br /><br />

### 5. 예제
```javascript
function milliseconds(x) {
  if (isNaN(x)) {
    return 'Not a Number!';
  }
  return x * 1000;
}

console.log(milliseconds('100F'));
// expected output: "Not a Number!"

console.log(milliseconds('0.0314E+2'));
// expected output: 3140
```
