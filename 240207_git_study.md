#GitStudy

- git .md 파일 만들기
1. echo "글" >> 파일명.md

- git add와 commit 을 한번에 
1. git commit -am ""

- git branch 만들기 
(브랜치는 분기된 차원으로 프로젝트를 하나이상의 버전으로 관리할 때 사용 : 실배포용, 테스트 서버용 등 )
1. git branch 브랜치명
2. git branch(branch 목록 확인)
3. git switch 다른 브랜치명 (브랜치로 이동 )
4. git switch -c (신규브랜치 생성 및 이동)
5. git branch -d 브랜치명(브랜치 삭제)
6. git branch -m 기존브랜치명 새로운브랜치명 ( 브랜치명 변경)
7. git log --all--decorate --oneline --graph (브랜치의 내역 확인)
