# substring
### 1. 요약
문자열에서 특정한 구간의 문자열을 추출
<br /><br />

### 2. 문법
```javascript
string.substring(from,to)
```
<br />

### 3. 인자
|인자명|데이터형|필수/옵션|설명|
|---|---|---|---|
|from|number|필수|탐색구간의 시작점(index)|
|to|number|옵션|탐색구간이 끝나는 점, 0 index 부터 시작|
<br />

### 4. 반환값
string, from과 to 사이의 문자열
<br /><br />

### 5. 설명
from이 to 보다 **작으면** from부터 to사이의 문자열을 리턴.  
from이 to 보다 **크면** to부터 from 사이의 문자열을 리턴.  
from과 to가 **같으면** 빈문자열을 리턴.  
<br /><br />

### 6. 예제
```javascript
let str1 = "banana";
let str2 = str1.substring(0, 4);
console.log(st2);

// expected output: bana
```
