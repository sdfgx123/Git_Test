# Git_Test
깃허브 명령어 숙달 및 테스트를 목적으로 만든 리포지토리

## 목적
01. Git reset과 revert의 명확한 구분 및 테스트
02. .gitignore 파일 사용법 및 테스트
03. Git branch 사용법 및 branch 간 
<br>
## 최근 특이사항
1. (04/01) 로컬 저장소에서 commit 까지만 한 뒤, # git reset {바로 이전 Hash}를 통해 commit 내용을 되돌리려 했으나 워킹 디렉토리까지 날아가 버림.
1.1. 다른 블로그에서 찾아봤을 때 # git reset에서 옵션 안 주면 --mixed가 default라서 워킹 디렉토리는 안 날라갈 줄 알았는데 날라가 버림. > 이 부분 재현해서 테스트

2. (04/01) 외부 저장소 fork > clone > add > commit > push > pull request > 실수로 merge > 변경사항 rm으로 삭제(원복) 후 다시 merge > 정상 pull request 함
2.1. # git reset --hard {이전 해쉬} > # git force push을 해결방법으로 들음 > 재현 후 다시 테스트 예정
