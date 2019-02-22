# git
  - git init
    - git initialize repository
  - git add 
    - add to staging area
    - git add * 는 전부 스테이지에 올림.
    - git add . 현재 모든디렉터리
    - git add ./src  지정된 src 디렉토리만,
  - git status
    - working tree status
  - git commit -m ""
    - create version
  - git commit -am ""
    - 한번은 tracked 되어야한다. 
    - add와 commit 동시 
  - (커밋 후) git log
    - show version
    - 커밋후 git log 하면 커밋내용 보여짐
  - git log --stat
    - show file change
  - git diff
    - show changes
   - git log - p
    - patch 
    - 파일 변경이력을 한번에 보기

   - git checkout ~~
     -  ~~ 는 git log해서 봤을때 나오는 comit 뒤의 key값
     -  그때 버전으로 돌아가기 (HEAD를 그쪽으로 옮기기== git checkout master)
     -  git checkout master는 가장 최신버전(최근커밋)으로 돌아가기.


# git posix text editor 바꾸기

   - git config --global core.editor "nano" 
     - git commit 시에 맨위에 적으면됌.


# revert (살려두고 커밋으로 되돌아가기)
- git revert 전단계커밋 key
- <b>(!important)</b>바로 전단계것을 revert해야한다. 
- 전단계는 살아있고 돌아감. reset보다 권장.

# reset (완전제거)
- 전 버전 다지우고 돌아가기.
- git reset --hard (git log commit뒤에 버전)
- commit뒤에 버전이 되어있음.

