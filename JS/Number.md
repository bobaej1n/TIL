# Number
### 1. 요약
숫자(원시 숫자 자료형)를 다룰 때 유용한 프로퍼티와 메소드를 제공하는 레퍼(wrapper) 객체
<br /><br />

### 2. 문법
```javascript
new Number(value)
```
<br />

### 3. 설명
변수 또는 객체의 프로퍼티가 숫자를 값으로 가지고 있다면 Number 객체의 별도 생성없이 Number 객체의 프로퍼티와 메소드를 사용할 수 있다.
<br /><br />

### 4. 예제
```javascript
var num1 = new Number(1);
var num2 = Number.MAX_SAFE_INTEGER; // 안전하게 변수 초기화하는 방법
var num3 = Number.MIN_SAFE_INTEGER;
```
