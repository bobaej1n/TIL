# zsh: command not found: brew 오류
### 1. 오류
```bash
zsh: command not found: brew
```
</br>

### 2. 원인
Homebrew가 /usr/local/... 가 아닌  /opt/homebrew/ 에 설정되어 있기 때문.
<br /><br />

### 3. 해결 방법
```bash
vi ~/.zshrc
```
로 들어간 후
```bash
export PATH=/opt/homebrew/bin:$PATH
```
홈 디렉토리의 .zshrc 로 설정해 ZSH shell이 brew command를 찾아 실행할 수 있다.