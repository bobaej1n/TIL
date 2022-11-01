# push
### 1. 요약
배열에 값을 추가함. 추가된 배열은 마지막 원소가 됨
<br /><br />

### 2. 문법
```javascript
array.push(element1, element2, ..., elementN)
```
<br />

### 3. 인자
|인자명|데이터형|필수/옵션|설명|
|---|---|---|---|
|elementN|all|필수|배열의 마지막 원소로 추가될 데이터|
<br />

### 4. 반환값
원소가 추가된 이후에 배열의 원소 수(length)
<br /><br />

### 5. 설명
array.unshift()는 반대의 기능.  
원본 데이터의 값이 변경된다.
<br /><br />

### 6. 예제
```javascript
var arr = ['bo', 'bae'];
var jin = jobs.push('jin');
alert(jin); // number, 3
alert(arr); // array, ['bo', 'bae', 'jin'], 원본 arr의 값이 변경 되었다.
```
