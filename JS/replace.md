# replace
### 1. 요약
문자열을 다른 문자열로 치환한 결과를 리턴
<br /><br />

### 2. 문법
```javascript
string.replace(regexp|substr, newSubStr);
```
<br />

### 3. 설명
문자열에서 주어진 패턴(regexp|substr)에 해당하는 부분을 새로운 데이터(newSubStr)로 치환 후 반환.  
인자로 주어진 값(newSubstr)은 변하지 않음.
<br /><br />

### 4. 예제
```javascript
let str1 = "banana";

// 문자를 이용해서 값을 치환
let str2 = str1.replace('a', '#');  // expected output: b#nana
//replaceAll: 해당 하는 문자 모두 치환함.
str2 = str1.replaceAll('a', '#'); // expected output: b#n#n#
```