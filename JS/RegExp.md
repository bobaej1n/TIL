# 정규표현식(Regular Expression, RegExp)
### 1. 요약
문자열에서 특정 문자 조합을 찾기 위한 패턴
<br /><br />

### 2. 문법
```javascript
/pattern/(g)
```
g: global → 해당 문자열에서 모두 찾아라(option)
<br /><br />

### 3. 설명
정규 표현식도 객체로서, RegExp의 exec()와 test() 메서드를 사용할 수 있음. String의 match(), matchAll() (en-US), replace(), replaceAll() (en-US), search(), split() 메서드와도 함께 사용할 수 있음.
<br /><br />

### 4. 예제
```javascript
let str1 = "banana";
let str2 = str1.replace(/a/g, '#')  // expected output: b#n#n#
```