# 로컬 변경 사항을 원격 저장소에 푸시하기
> 변경사항을 서버에 올려서 다른 사람도 볼 수 있게 하는 작업이다.

![push](../images/BasicPush.png)

1. `git push -u origin [브랜치 이름]`
   * 아무 경고가 뜨지 않으면 완료된 것이다! 이때는 GitHub에 들어가 변경사항이 잘 업로드되었는지 확인한다.
   * 다음과 같은 경고가 뜨면서 실패하는 경우가 있다.
     * 메시지 예:
      ```
      error: failed to push some refs to '[레포지토리 주소]'
      hint: Updates were rejected because the remote contains work that you do
      hint: not have locally. This is usually caused by another repository pushing
      hint: to the same ref. You may want to first integrate the remote changes
      hint: (e.g., 'git pull ...') before pushing again.
      hint: See the 'Note about fast-forwards' in 'git push --help' for details.
      ```
     * 이 경우에는 [원격 저장소의 변경 사항을 로컬로 가져오기](pull.md)의 명령어를 입력한다.
   * `-u` 옵션의 의미는 [여기](https://wotres.tistory.com/entry/git-push-u-%EC%98%B5%EC%85%98-%EC%82%AC%EC%9A%A9-%EC%9D%B4%EC%9C%A0) 참조
   * 잘못된 커밋이 있는 경우 절대 `git push`하지 말고 로컬에서 커밋을 조작하는 것을 추천한다.
     * 지난 커밋을 조작하는 방법은 여기서 다루지 않는다. 검색해서 찾아보기를 바란다.
