# oss 깃허브 교과목 내용 정리 📒 
## 깃 설정
$ git config --global user.name ---- 사용자 이름

$ git config --global user.email ----@gmail.com 사용자 전자메일

$ git config --global core.autocrlf true 줄바꿈 자동변환

$ git config --global core.safecrlf false 줄바꿈 안전 설정

$ git config --global core.editor 'code --wait' 기본 편집기 설정

$ git config --global init.defaultBranch main 기본 브랜치 이름

# 깃 repository 설정

$ git init
   현재 디랙토리를  git repository로 만들기 위해 사용

$ git init basic 
   현재  폴더 하부에 basic을 생성하고 git repository로 만들기 위해서 사용

# 깃커밋과 로그
## 깃상태보기
$ git status[--long]  현재의 상태 표시
$ git status[--short|-s]   현재의 상태를 간단히 표시
$ git config --global --edit  도움말 보기


## 커밋 로그 이력보기
$ git log  로그이력 정보를 표시
$ git log --oneline 로그 이력을 한줄로 표시
$ git log[--patch|-p] 로그 이력과 함께 파일의 변화를 표시

## 커밋정보 git show 
$ git show 마지막 커밋의 커밋정보 표시
$ git show --oneline 커밋 로그 한줄과 파일차이 표시
$ git show -s 파일 차이는 표시되지 않음
$ git show [HEAD] 지정한 head의 커밋 정보 표시
$ git show [commitID]지정한 commitID의 커밋정보 표시

## 원격저장소 복제 연동
$ git pull origin main 원격저장소 수정사항 pull로 지역 저장소로 가져오기
$ git fetch 원격저장소 수정사항 fetch로 지역 저장소로 가져와 병합하기
$ git push origin main  원격저장소 수정사항 push로 원격저장소로 보내기

# 파일삭제 rm과 복원 restore
$ rm f 작업디랙토리에서 파일 삭제
$ git rm f 작업 디랙토리와 스테이지 영역에서 파일 삭제
$ git rm --cached f 스테이징영역에서만 파일 삭제
$ git restore f 스테이징영역 상태를 작업 디랙토릭에 복원 
