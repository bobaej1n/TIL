# substr
### 1. 요약
문자열에서 특정한 구간의 문자열을 추출
<br /><br />

### 2. 문법
```javascript
string.substr(start,length)
```
<br />

### 3. 인자
|인자명|데이터형|필수/옵션|설명|
|---|---|---|---|
|start|number|필수|탐색구간의 시작점(index)|
|length|number|옵션|	탐색구간이 끝나는 점(index), start+length 위치까지를 탐색구간으로 설정함|
<br />

### 4. 반환값
string, start와 length 사이의 문자열
<br /><br />

### 5. 설명
문자열 중 첫번째 인자(start)에서부터 두번째 인자(length)까지의 구간에 해당하는 문자열을 반환함.  
length를 지정하지 않으면 start에서부터 문자열 전체를 처리구간으로 간주함.  
start가 양수일 경우, 문자의 길이 보다 작으면 빈문자열이 리턴됨.  
start가 음수일 경우, start의 index는 문자열의 뒤에서부터 시작됨.  
<br /><br />

### 6. 예제
```javascript
var str = 'coding everybody';
alert(str.substr(7)) // everybody
alert(str.substr(7,5)) // every
alert(str.substr(-4)) // body, 음수인 경우 뒤에서부터 카운팅 alert(str.substr(-4,2)) // bo
alert(str);
```
