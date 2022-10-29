# concat
### 1. 요약
복수의 배열을 결합해서 리턴
<br /><br />

### 2. 문법
```javascript
array.concat(value1, value2, ..., valueN)
```
<br />

### 3. 인자
|인자명|데이터형|필수/옵션|설명|
|---|---|---|---|
|valueN|array|필수|결합할 배열|
<br />

### 4. 반환값
string 과 valueN을 결합한 Array
<br /><br />

### 5. 설명
원본 데이터의 값을 변경하지 않음.
<br /><br />

### 6. 예제
```javascript
var a = new Array(1,2,3);
var b = new Array(4,5,6);
var c = new Array(7,8,9);
 
a.concat(b,c); // [1,2,3,4,5,6,7,8,9]
```
