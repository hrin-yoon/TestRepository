#GitStudy

>>> git bash 설치
  
- 로컬 저장소로 들어가기
  1. cd rin_project
  2. git init
 
- 원격 저장소 연결하기
  1. git remote add "원격저장소주소"
-  만약 원격 저장소 위치를 바꿀 경우
  1. git remote origin remove
     
- 원격 저장소 파일 업로드/ 수정 후 다시 업로드시 (로컬 -> 원격)
  1. git status
  2. git add . 또는 git add <파일명>
  3. git commit -m "메세지"
  4. git push

- 원격 저장소에 있는 파일 변경후 로컬로 반영 (원격 -> 로컬)
  1. git remote update
  2. git stash
  3. git pull

<<<<<<< HEAD
- 로컬 저장소 파일 특정 버전으로 되돌리기
  1. git log (해쉬번호 확인/ 빠져나오기 q)
  2. git reset --hard 해쉬
=======

이건 되돌리기를 위한 방법이다이. (이거 삭제)
이것도 알지 ?
>>>>>>> dcd04cde5c5d5c95102dc32c254bee8c7a209b39
