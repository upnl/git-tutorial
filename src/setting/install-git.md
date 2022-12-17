# 설치

Git을 사용하려면 우선 설치를 하여야 한다. 이는 다음과 같이 크게 3가지 방법으로 설치할 수 있다.

* 패키지 관리자를 사용하여 설치
* 별도의 바이너리 인스톨러를 받아 설치
* 직접 소스코드를 내려받아서 컴파일

패키지 관리자를 사용하여 설치하는 것이 가장 간편하고 보편적인 방법이다. 따라서 여기에서는 이 방법을 사용하여 설명을
진행한다. 나머지 두 방법의 경우 여기서 다루지 않으니 필요한 경우 직접 알아볼 것을 추천한다.

## Windows
윈도우는 Windows 10 버전 1709부터 공식 패키지 관리자인 `winget` 을 지원한다.

```console
$ winget install -e --id Git.Git
```

## Linux
각 리눅스 배포판에서 제공하는 패키지 관리자를 사용하면 된다. 다음은 그 예시이다.

### Debian/Ubuntu

```console
$ apt install git
```

### Arch Linux

```console
$ pacman -S git
```

### Nix/NixOS

```console
$ nix-env -i git
```

### Alpine

```console
$ apk add git
```

## macOS

macOS의 경우 기본적으로 개발 환경 구성을 위해 Command Line Tools for Xcode를 설치하여야 하는데, 이 때 Git이 자동으로
설치가 된다. 이는 다음과 같이 입력하여 설치할 수 있다. 이 과정은 macOS 버전을 업데이트 시 다시 진행할 필요가 있다.

```console
$ xcode-select --install
```
