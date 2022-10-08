# splice
### 1. 요약
배열의 특정구간을 추출하거나, 특정구간에 특정 배열을 추가함
<br /><br />

### 2. 문법
```javascript
array.splice(index, howmany, element1, ...., elementN);
```
<br />

### 3. 인자
|인자명|데이터형|필수/옵션|설명|
|---|---|---|---|
|index|number|필수|배열에 추가할 특정 배열의 위치를 가르키는 index|
|howmany|number|필수|index에서부터 제거될 원소들의 수. index부터 index+howmany에 해당하는 원소들은 삭제됨. 이 값이 0이면 어떠한 원소도 삭제되지 않음.|
|element1,...,elementN|number|옵션|index와 index+howmany 사이에 추가될 값|
<br />

### 4. 반환값
array, index와 index+howmany 사이에 해당하는 원소들을 패키징한 배열
<br /><br />

### 5. 설명
배열에 배열을 추가하거나, 삭제할 때 사용. 대상 구간에 해당하는 삭제될 원소들은 리턴됨.  
원본이 수정됨. slice가 원본이 유지되는 것과 다름.
<br /><br />

### 6. 예제
```javascript
var numbers = [1,2,3,4,5,6,7,8,9,10];
alert(numbers.splice(2)); // array, [3,4,5,6,7,8,9,10], 시작점 2부터 배열의 마지막 원소까지를 대상으로 함.
alert(numbers); // array, [1,2], 원본이 수정됨.
 
var numbers = [1,2,3,4,5,6,7,8,9,10];
alert(numbers.splice(2, 4)); // array, [3,4,5,6]
 
var numbers = [1,2,3,4,5,6,7,8,9,10];
alert(numbers.splice(2, 4, 'three', 'four', 'five', 'six')); // array, [3,4,5,6]
alert(numbers); // array, [1,2,three,four,five,six,7,8,9,10]

```
