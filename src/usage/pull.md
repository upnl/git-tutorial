# 원격 저장소의 변경 사항을 로컬로 가져오기
![pull](../images/BasicPull.png)
1. `git fetch origin`
   * 원격 레포지토리의 변경사항이 로컬 레포지토리에 반영된다.
2. `git pull origin [현재 브랜치 이름]` 또는 간단히 `git pull`
   * 원격 레포지토리의 변경사항이 로컬 작업 환경에 반영된다.
     * Git 설치 시 기본 세팅에서 "rebase" 옵션을 선택했다면([설치 문서](../install/binary.md)를 그대로 따라갔다면) 자동으로 `git pull --rebase` 방식으로 동작한다.
     * 만약 pull의 기본 동작이 rebase로 동작하지 않는다면 `git config --global pull.rebase true`를 입력하여 설정할 수 있다.
     * rebase와 관련한 내용은 이 문서에서는 자세히 다루지 않겠다.
   * 가끔 merge conflict가 뜨면서 이 명령이 실패하는 경우가 발생한다.
      * 메시지 예:
       * `CONFLICT (content): Merge conflict in [파일 이름]`
       * `Automatic merge failed; fix conflicts and then commit the result.`
     * 이것은 두 명 이상의 사람이 같은 시기에 특정 파일의 특정 부분을 서로 다르게 변경하여 발생하는 충돌이다.
     * 이때는 [머지 컨플릭트 해결법](merge-conflict.md)을 수행한다.
     * 특히 Unity를 사용할 때 같은 scene을 둘 이상의 사람들이 동시에 변경해서 머지 컨플릭트가 발생하게 되면 다른 파일들보다 해결하기 어렵기 때문에 가급적 scene 파일은 한 번에 한 사람만 수정하는 것으로 한다.
   * 현재 브랜치 이름 대신 다른 브랜치 이름을 입력해서 `git pull origin [다른 브랜치 이름]`을 수행하는 경우, `다른 브랜치`가 `현재 브랜치`에 merge된다.
     * `git merge`에 익숙하지 않다면 이것을 하는 것을 추천하지 않는다.
     * 헷갈린다면 그냥 `git pull`을 하자.
3. push를 하려던 중이었다면 다시 [로컬 변경 사항을 저장하기](commit.md)부터 하나씩 실행한다.
