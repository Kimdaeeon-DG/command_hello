remote repository of git_tutorial

2024.04.14

1. git tag
-> git tag 1.0 // tag를 1로 설정
-> git log -3  // 로그를 3개 보겠다. (숫자만큼 나옴)
-> git show-ref --tags  // tag들의 주소와 태그를 다 보겠다.
-> git tag -a 0.8 3889  // commit 주소의 앞자리 4개를 적고 태그를 0.8로 설정 후 추가적으로 메모하겠다. (빔에디터로 들어가짐)
-> git tag -l // 태그들 이름만 다 나옴
   
3. git commit --amend
-> git commit --amend // 이렇게 하면 vim으로 들어가서 바꿀 수 있음.

4. git revert
-> git revert 7480 

5. git reset // 해당 점으로 돌아가되, 돌아가는 내용의 커밋을 새로 만들고 그 전 커밋을 지우지느 않음.
-> git reset --soft HEAD~~~  // soft는 저장소를 바꾸지 않음. 그리고 HEAD뒤에 물결 표시 갯수만큼 돌아가겠다는거임. (3개 돌아감)
-> git reset --hard HEAD~~~  // hard는 저장소를 바꿈. 그리고 HEAD뒤에 물결 표시 갯수만큼 돌아가겠다는거임. (3개 돌아감)
-> git reset --hard ORIG_HEAD // 아까 한 행위를 복구하겠다. soft로 했을 때는 hard 자리에 soft 넣으면 됨.
   
7. git checkout HEAD filename
-> git checkout HEAD -- README.md // checkout은 해당 지점 커밋으로 돌아감. 그리고 그 전의 커밋 내용을 다 지움.
