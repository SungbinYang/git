# git

## 버전관리(VCS)

### 1. 개행문자 설정 
  * $ git config --global core.autocrlf input ( 개행 문자 설정 :: MAC 기준 )
  * $ git config --global core.autocrlf true ( 개행 문자 설정 :: Windows 기준 )

### 2. 사용자 정보, 커밋(버전 생성)을 위한 정보 등록
  * $ git config --global user.name 'YOUR_NAME'
  * $ git config --global user.email 'YOUR_EMAIL'
  * 여기서 사용자 이름은 아무거나 지정해도 되지만 되도록 깃에 등록한 이름으로 하는것이 좋다.

### 3. 구성확인
  * $ git config --global --list 
  * 종료할려면 Q키를 눌러서 종료

### 4. 현재 프로젝트에서 변경사항 추적(버전 관리)을 시작
  * $ git init

### 5. 변경사항을 추적할 특정 파일(index.html)을 지정
  * $ git add index.html // stage로 index.html파일이 올라간다.
  * $ git add . // 모든 파일의 변경사항을 추적하도록 지정

### 6. 메세지(-m)와 함꼐 버전을 생성
  * $ git commit -m 'YOUR_PROJECT'

### 7. origin이란 별칭으로 원격저장소를 연결
  * $ git remote add origin <span>https://github.com..... .git</span>

### 8. origin이란 별칭의 원격 저장소로 버전 내역 전송
  * $ git push origin master

### 9. 프로젝트 복제
  * $ git clone 원격 repository 주소

### 10. branch
  * $ git branch // 현재 브랜치 정보를 보여준다.
  * $ git branch -a // 깃허브의 원격저장소에 있는 브랜치 정보도 알수 있다.
  * $ git branch 새로운 브렌치 이름 // 새로운 브렌치 생성
  * $ git checkout 새로만든 브랜치 이름 // 새로만든 브랜치로 접속한다.

### 11. git의 상태 및 로그 확인
  * $ git status // 깃의 변경된 사항을 확인한다. 수정사항이 있으면 빨간색으로 수정사항이 있는 파일이 나오고 git add .을 완료하고 보면 파란색으로 바껴있는것을 확인할수 있다.
  * $ git log // 깃의 로그를 확인한다. 변경사항의 히스토리를 알수 있다.

### 12. 이전 버전으로 돌리는 법
  * $ git reset --hard HEAD~1 // 이전버전으로 완벽히 돌려준다. HEAD의 최신버전에서 뒤로 한 버전 되돌린다
  * $ git reset --hard ORIG_HEAD // 되돌리기를 잘못해서 그것을 취소하려는 경우; 다음 명령을 입력하기 전까지 1번은 할 수 있다

### 13. branch 가져오기 및 삭제
  * $ git branch -r // 원격저장소에 있는 branch들의 목록을 확인할수 있다
  * $ git checkout -t 별칭/브랜치 이름 // 원격저장소에 branch를 로컬환경으로 가져온다.
    * ex) $ git checkout -t origin/purple 
  * $ git branch -d branch 이름 // 브랜치 삭제
  * $ git branch -b branch 이름 // 브랜치 생성 및 이동

### 14. 충돌, 로컬병합
  * $ git pull origin master // 원격저장소 master브랜치를 로컬저장소로 당겨온다
  * 충돌이 날 경우 위의 명령어를 작성 후, vscode같은 경우 에디터의 힘으로 현재요청을 받아들일지 아님 수신변경 사항을 가르킬지 사용자가 선택할수 있으며 이 2개가 전부 아닌 새로운 사항을 작성할 수 있다.


# MarkDown

### 1. 장점
 * 문법이 쉽고 간결하다
 * 관리가 쉽다
 * 지원가능한 플랫폼과 프로그램이 다양하다

### 2. 단점
 * 표준이 없다!
 * 모든 HTML 마크업을 대신하지 못한다.
