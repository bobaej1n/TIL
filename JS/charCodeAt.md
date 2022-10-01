# charCodeAt
### 1. 요약
index에 해당하는 문자의 unicode 값을 리턴
<br /><br />

### 2. 문법
```javascript
string.charCodeAt(index)
```
<br />

### 3. 인자
index - 필수, 0보다 큰 정수
<br /><br />

### 4. 설명
charCodeAt은 주어진 index에 해당하는 유니코드 값을 리턴하는데 이 값은 unicode가 지원되는 모든 시스템에서 동일한 문자를 가르킴.  
charAt 는 index에 해당하는 문자를 리턴하고, chartCodeAt은 유니코드 값을 리턴하는 차이가 있음.
<br /><br />

### 5. 예제
```javascript
let c = "a"
let num = c.charCodeAt();
console.log(num);

// 알파벳 대문자: 65~90
// 알파벳 소문자: 97~122
// expected output: 97
```
