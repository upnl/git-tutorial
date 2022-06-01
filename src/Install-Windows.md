## Git 설치
* [이전으로 돌아가기](./README.md#설치)
### Windows
1. [여기](http://git-scm.com/download/win)에서 "Click here to download" 링크 클릭
2. 다운로드한 파일 실행
  * 아래는 버전 2.35.1.2-64-bit 및 2.36.1-64-bit 기준으로 작성하였다. 최신 버전이 있다면 최신 버전을 받으면 된다.
3. ![설치1](Screenshots/%EC%84%A4%EC%B9%981.PNG)
  * "Only show new options"를 체크하지 **않고** "Next" 클릭
4. 설치 경로 지정
5. ![설치2](Screenshots/%EC%84%A4%EC%B9%982-1.PNG)
  * 위 사진처럼 체크하고 "Next" 클릭
    * Windows Explorer integration 체크
      * Git Bash Here 체크
      * Git GUI Here 체크
    * Git LFS (Large File Support) 체크
    * Associate .git* configuration files with the default text editor 체크
    * Associate .sh files to be run with Bash 체크
    * (NEW!) Add a Git Bash Profile to Windows Terminal **체크**
  * 다른 옵션도 읽어보고 필요하면 체크해도 괜찮다.
6. 시작 메뉴에 폴더 만들 것인지 묻는 창이 뜬다면, "Next" 클릭
7. ![설치3](Screenshots/%EC%84%A4%EC%B9%983.PNG)
  * **Visual Studio Code**가 설치되어 있는 경우 위 사진처럼 Code를 사용할 수 있고, 아니면 메모장(Notepad)이나 본인이 편한 에디터(Vim 등)로 설정하면 된다.
  * 나중에 커밋 메시지를 작성하거나 머지 커밋이 발생할 때 여기서 설정했던 에디터가 열린다.
8. ![설치4](Screenshots/%EC%84%A4%EC%B9%984.PNG)
  * 위 사진처럼 **두 번째 항목에 체크**하고 초기 브랜치 이름이 `main`으로 적혀 있는지 확인하고 "Next" 클릭
  * 현재 GitHub의 주 브랜치 이름의 기본값은 `main`이다.
    * 예전에는 새 레포지토리의 주 브랜치 이름이 `master`였다.
  * 이미 Git을 사용하고 있었다면, 이 옵션을 변경하여 새로 설치해도 기존 레포지토리에는 영향을 주지 않는다.
9. ![설치5](Screenshots/%EC%84%A4%EC%B9%985.PNG)
  * 중간에 "(Recommended)"된 두 번째 항목에 체크하고 "Next" 클릭
10. ![설치6](Screenshots/%EC%84%A4%EC%B9%986.PNG)
  * 위 사진처럼 첫 번째 항목에 체크하고 "Next" 클릭
11. ![설치7](Screenshots/%EC%84%A4%EC%B9%987.PNG)
  * 위 사진처럼 첫 번째 항목에 체크하고 "Next" 클릭
12. ![설치8](Screenshots/%EC%84%A4%EC%B9%988.PNG)
  * Windows 사용자라면 위 사진처럼 첫 번째 항목에 체크하고 "Next" 클릭
13. ![설치9](Screenshots/%EC%84%A4%EC%B9%989.PNG)
  * 위 사진처럼 첫 번째 항목에 체크하고 "Next" 클릭
  * 그러나 명령 프롬프트(cmd)를 너무나 사랑한다면 두 번째 항목에 체크하고 "Next" 클릭해도 된다. (비추천)
14. ![설치10](Screenshots/%EC%84%A4%EC%B9%9810-1.PNG)
  * 위 사진처럼 **두 번째 항목에 체크**하고 "Next" 클릭
    * `git pull` 명령 사용 시 자동으로 `git pull --rebase` 명령을 사용한 것과 동일하게 처리한다.
    * 머지 커밋이 불필요하게 쌓이는 것을 방지하기 때문에 추천한다.
  * 머지 커밋을 남겨도 상관없는 경우 첫 번째 항목에 체크하고 "Next" 클릭
    * 사람에 따라 머지 커밋이 기록으로 남는 게 지저분하다고 생각할 수 있다. 그러나 사실 그렇게 중요한 문제는 아니다.
15. ![설치11](Screenshots/%EC%84%A4%EC%B9%9811.PNG)
  * 위 사진처럼 첫 번째 항목에 체크하고 "Next" 클릭
16. ![설치12](Screenshots/%EC%84%A4%EC%B9%9812.PNG)
  * 위 사진처럼 첫 번째 항목에만 체크하고 "Next" 클릭
17. ![설치13](Screenshots/%EC%84%A4%EC%B9%9813.PNG)
  * 위 사진처럼 아무 항목도 체크하지 **않고** "Install" 클릭
  * 각 항목을 읽어보고 써보고 싶다는 생각이 들면 체크해도 괜찮다.