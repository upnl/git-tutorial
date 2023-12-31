# Git 설정
터미널을 세팅한 후 Git을 설치하였으면 이제 Git 명령어를 칠 준비가 된 것이다.
하지만 실제로 Git을 사용하려면 사용자 정보나 몇 가지 환경 설정을 더 할 필요가 있다.

기본적으로 Git의 설정은 다음 두 파일에서 값을 읽고 수정하여 진행할 수 있다.

* 현재 사용자에게 적용되는 설정인 `~/.gitconfig`
* 현재 디렉토리에만 적용되는 설정인 `.git/config`

설정 파일은 `.git/config` 파일이 `~/.gitconfig` 파일보다 우선시 된다.

## Git 설정하기

앞에서 언급한 파일을 수정하여도 무방하지만, 여기서는 `git config` 명령어를 사용하여 설정을 진행한다.
터미널을 실행한 후 다음 과정을 진행한다.

### 사용자 정보

Git을 설치한 후 가장 먼저 할 일은 사용자 이름과 이메일 주소를 설정하는 것이다.
다음과 같이 입력하여 사용자의 정보를 설정한다. `[your_name]` 및 `[you@example.com]` 부분에 자신의 이름과 이메일을 적으면 된다.

```console
$ git config --global user.name "[your_name]"
$ git config --global user.email "[you@example.com]"
```

> `--global` 옵션은 현재 사용자의 모든 리포지토리에 같은 아이덴티티를 적용하겠다는 의미이다.
> 만약 작업 중인 리포지토리에만 이 아이덴티티를 적용하고 싶다면 `--global` 대신 `--local` 옵션을 적어 실행한다.

### 기본 브랜치 이름

Git은 원래 기본 브랜치 이름으로 `master`라는 이름을 사용하였으나, 현재의 Git 생태계는 `main`이라는 이름을 사용하는 것을
권장한다. 따라서 다음과 같이 기본 브랜치 이름을 `main`으로 지정한다.

```console
$ git config --global init.defaultBranch main
```

### Git Pull 기본 동작

Git에서는 원격에서 업데이트가 된 데이터를 로컬에 반영할 때 `git pull` 명령어를 사용한다. 하지만 이 명령어의 기본 동작은
Pull의 동작을 정확히 이해하지 못한 채 사용해서는 안된다. 정석은 `ff-only` 모드를 사용하는 것이지만, 여기서는 편의상
defalut 모드를 사용한다. 자세한 내용은 [공식 문서](https://git-scm.com/book/ko/v2/Git-%EB%B8%8C%EB%9E%9C%EC%B9%98-Rebase-%ED%95%98%EA%B8%B0) 또는 [한글 문서](https://sanghye.tistory.com/43)를 참조하기 바란다.

## 설정 확인

`git config --list` 명령을 실행하면 설정한 모든 것이 보여진다. 이는 설치법이나 세팅에 따라 다음 예시보다 추가적인 항목이 더 있을 수 있다.

```console
$ git config --list
user.email=[REDACTED]
user.name=[REDACTED]
init.defaultBranch=main
```
