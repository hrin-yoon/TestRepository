#GitStudy

- git 명령어 초기화
1. git init 

- git .md 파일 만들기
1. echo "글" >> 파일명.md

- git add와 commit 을 한번에 
1. git commit -am ""

- github 에서 새로운 프로젝트 다운 
1. git clone 프로젝트원격주소

Git branch ? 
개발을 하다보면 코드를 여려개로 복사해야 하는 일이 자주 발생한다. 브랜치는 원래 코드와 상관없이 독힙적으로 개발을 진행 할 수 있도록 해준다. 협업시 사용할 경우 좋음 
(브랜치는 분기된 차원으로 프로젝트를 하나이상의 버전으로 관리할 때 사용 : 실배포용, 테스트 서버용 등 )

HEAD?
모든 브랜치에 HEAD 값이 존재하는데 HEAD란 해당 브랜치의 마지막 commit을 뜻한다. -> 마지막 commit의 포인트 

- 로컬과 원격의 브랜치를 전부확인할 수 있음 
1. git branch -a 
2. git branch -all 

- git branch 만들기 
1. git branch 브랜치명
2. git branch(branch 목록 확인)
3. git switch 다른 브랜치명 (브랜치로 이동 )
4. git switch -c (신규브랜치 생성 및 이동)
5. git branch -d 브랜치명(브랜치 삭제)
6. git branch -m 기존브랜치명 새로운브랜치명 ( 브랜치명 변경)
7. git log --all--decorate --oneline --graph (브랜치의 내역 확인)

- git branch merge (브랜치 합병 )
(두 브랜치를 한 커밋에 이어붙이는 방식/ 브랜치의 사용내역을 남길 필요가 있을 때)
#합쳐져서 주요 브랜치가 될 브랜치로 이동 
#merge는 reset으로 되돌리기가 가능함. merge하기 전 해당 브랜치의 마지막 시점으로 reset
1. git switch main
2. git merge add-합칠 브랜치명 

- 병합된 브랜치 삭제
1. git branch -d add-삭제할 브랜치 명 

- Rebase 브랜치를 다른 브랜치에 이어붙이는 방식 
(여러개의 브랜치가 아닌 하나의 줄로 깔끔히 정리)
#이미 팀원들과 공유한 커밋에 대해서는 사용하지 않는 것이 좋음
#merge와 반대로 합쳐질 브랜치로 이동 
1. git switch 합쳐질 브랜치명 
2. git rebase main

#new-teams 브랜치가 main에 합쳐졌지만 아직 main은 new-teams 브랜치의 끝에 있지 않다.
#따라서 main 브랜치로 이동 후 new-teams의 시점으로 fast-forward해준다
1. git merge new-teams

- 합친 브랜치 삭제
1. git branch -d new-teams

- 로컬의 branch를 원격 저장소로 push
1. git push --set-upstream orgin "브랜치명"
