# split
### 1. 요약
문자열을 인자로 주어진 문자열을 기준으로 쪼개서 배열에 담음
<br /><br />

### 2. 문법
```javascript
string.split(separator, limit)
```
<br />

### 3. 반환값
array, 첫번째 인자(separator)를 기준으로 분리된 문자열들을 원소로 가지고 있는 배열
<br /><br />

### 4. 예제
```javascript
var str = 'html,css,javascript,jquery';
str.split(',') // 배열 [html,css,javascript,jquery]
str.split(',', 2) // 배열 [html,css]
```
