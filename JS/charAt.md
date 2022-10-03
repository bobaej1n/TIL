# charAt
### 1. 요약
문자열에서 인자로 주어진 값에 해당하는 문자를 리턴
<br /><br />

### 2. 문법
```javascript
charAt(index)
```
<br />

### 3. 인자
index - 필수, 0보다 큰 정수
<br /><br />

### 4. 설명
charAt은 index로 주어진 값에 해당하는 문자를 리턴함.  
존재하지 않는 index를 인자로 전달하면 공백이 출력됨.  
charAt 는 index에 해당하는 문자를 리턴하고, chartCodeAt은 유니코드 값을 리턴하는 차이가 있다.
<br /><br />

### 5. 예제
```javascript
var s = 'coding';
alert(s.charAt(0)); // c
alert(s.charAt(s.length-1)); // g
alert(s.charAt(1000) == ''); // true
```
