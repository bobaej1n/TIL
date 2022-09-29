# String
### 1. 요약
문자열 객체
<br /><br />

### 2. 문법
```javascript
var 참조변수 = new String(문자열 데이터)
var 참조변수 = 문자열 데이터
```
<br />

### 3. 설명
String(문자열) object(객체)는 자바스크립트의 원시 데이터 형이다.  
자바스크립트에서는 String object를 생성하는 다양한 방법이 있는데 문법과 같이 new를 이용하는 것과 ", ' 를 이용하는 방법이 있다.
<br /><br />

### 4. 예제
```javascript
var a = new String('문자열');
var b = String('문자열');
var c = '문자열';
alert(a == b && b == c);
```
