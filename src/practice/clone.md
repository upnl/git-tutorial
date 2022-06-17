# 레포지토리 복제하기
* Git bash(Windows) 또는 터미널을 켠다.
  * [터미널 세팅](../setting/terminal.md) 참조
* `cd` 명령을 활용하여 레포지토리의 루트 폴더를 둘 상위 폴더로 이동한다.
* https://github.com/upnl/git-practice 에서 초록색 "Code" 버튼을 누르고 SSH 탭에 나타나는 주소를 복사한다.
* `git clone [레포지토리 SSH 주소]`를 입력한다.
  * `[레포지토리 SSH 주소]` 부분에 복사했던 주소를 붙여넣는다.
  * 비밀번호를 입력하라고 나오면 자신의 비밀번호를 입력한다.
>  * 참고: `git clone` 명령은 다음 명령들을 모두 입력한 것과 거의 비슷한 동작을 하는 명령이다.
>    * `git init`
>    * `git remote add origin [레포지토리 SSH 주소]`
>    * `git fetch origin`
>    * `git pull origin main`
>    * `git branch --set-upstream-to=origin/main main` (원격 브랜치 `main`를 자동으로 추적하도록 하는 명령)
>    * 추가로 원격 레포지토리에 있는 모든 브랜치를 자동으로 추적하도록 해준다.
>  * `git clone` 관련 공식 문서는 [여기](https://git-scm.com/docs/git-clone)를 참조
* `git clone` 과정이 완료되면 `git-practice`라는 폴더가 생성될 것이다.
  * `cd git-practice`를 입력해 폴더 안으로 이동한다.