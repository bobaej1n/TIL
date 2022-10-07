# indexOf
### 1. 요약
문자열 내에서 특정한 문자열의 index 값을 리턴
<br /><br />

### 2. 문법
```javascript
stringValue.indexOf(searchValue[,fromIndex])
```
<br />

### 3. 인자
|인자명|데이터형|필수/옵션|설명|
|---|---|---|---|
|searchValue|String|필수|탐색하고 싶은 문자열|
|fromIndex|Integer(0<fromIndex<stringValue.length-1)|옵션|탐색구간이 끝나는 지점|
<br />

### 4. 설명
stringValue에서 특정한 문자열의 위치(index)를 반환  
탐색하려는 문자열이 존재하지 않는다면 -1을 반환  
<br /><br />

### 5. 예제
```javascript
var stringValue = '자바스크립트';
alert(stringValue.indexOf('자바')); // 0
alert(stringValue.indexOf('스크립트')); // 2
alert(stringValue.indexOf('PHP')); // -1, PHP는 stringValue안에 존재하지 않음
```
