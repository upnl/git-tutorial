# 패키지 관리자를 사용하여 설치
Git은 운영체제에서 제공하는 패키지 관리자를 이용하여 설치할 수 있다.

## Windows
윈도우는 Windows 10 버전 1709부터 공식 패키지 관리자인 `winget` 을 지원한다.

```
winget install -e --id Git.Git
```

## Linux
각 리눅스 배포판에서 제공하는 패키지 관리자를 사용하면 된다.  
예를 들어 Ubuntu/Debian 의 경우 `apt` 을 이용한다.

```
sudo apt install git
```

## macOS
Mac은 기본적으로 개발을 하기 위해서는 Xcode를 설치해야 하는데, 이 때 Git이 자동으로 설치된다.  
필요한 경우 macOS 용 패키지 관리자인 `brew` 를 이용하여 설치할 수도 있다.

```
brew install git
```
