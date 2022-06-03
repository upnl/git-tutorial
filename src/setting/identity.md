# 계정 아이덴티티 설정
Git을 설치한 후 터미널을 세팅하였으면 이제 Git 명령어를 칠 준비가 된 것이다.  
하지만 Git을 사용하려면 몇 가지 환경 설정을 더 할 필요가 있다.

`git config` 로 설정 내용을 확인하고 변경할 수 있는데, 이는 다음 두 설정 파일에서 값을 읽어 가져온다.

* 현재 사용자에게 적용되는 설정인 `~/.gitconfig`
* 현재 작업 중인 프로젝트에만 적용되는 설정인 `.git/config`

설정 파일은 `.git/config` 파일이 `~.gitconfig` 파일보다 우선시 된다.

## 사용자 정보
Git을 설치한 후 가장 먼저 할 일은 사용자 이름과 이메일 주소를 설정하는 것이다.  
터미널을 실행한 후, 다음을 입력한다. `[you@example.com]` 부분을 자신의 이메일로 대체해서 적으면 된다.

```
`git config --global user.email "[you@example.com]"`
`git config --global user.name "[Your Name]"`
```

`--global` 옵션은 현재 사용자의 모든 레포지토리에 같은 아이덴티티를 적용하겠다는 의미이다.  
만약 이 레포지토리에만 이 아이덴티티를 적용하고 싶다면 `--global` 대신 `--local` 옵션을 적어 실행한다.

## 설정 확인
`git config --list` 명령을 실행하면 설정한 모든 것이 보여진다.  
설치법이나 세팅에 따라 다음 예시보다 추가적인 항목이 더 있을 수 있다.

```
$ git config --list
user.email=[REDACTED]
user.name=[REDACTED]
init.defaultbranch=main
pull.rebase=true
```
