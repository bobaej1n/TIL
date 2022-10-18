# join
### 1. 요약
배열의 원소를 결합해서 하나의 문자열로 만듦
<br /><br />

### 2. 문법
```javascript
array.join(separator);
```
<br />

### 3. 인자
|인자명|데이터형|필수/옵션|설명|
|---|---|---|---|
|separator|string|필수|배열의 원소를 하나의 문자열로 결합할 때 원소와 원소 사이에 위치할 문자열|
<br />

### 4. 반환값
string
<br /><br />

### 5. 설명
첫번째 인자(separator)로 배열의 원소를 결합해서 하나의 문자열을 만듦  
string.split와 반대되는 기능
<br /><br />

### 6. 예제
```javascript
var a = new Array("hello","world","!!");

// join의 첫번째 인자로 ' '를 전달했기 때문에 반환 값은 원소와 원소 사이에 공백이 들어간 결과가 반환된다.
alert(a.join(' ')); // string, hello world !!
```
