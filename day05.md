### .gitignore
(github)에서 특수한 파일로 README.md와 .gitignore가 있다.  
왠만해서는 이 두 파일은 무조건 만든다(고 한다).  

한번 버전 관리가 되기 시작한 파일은 나중에 .gitignore에 등록해도 버전 관리가 된다!  

.gitignore에서 지정한게 적용되는 것은 .gitignore가 저장된 시점부터..인 것 같다.  
그래서 .gitignore는 git init 시작하기 전에 만들어주세요  

```.gitignore
# : comments

# no .a files
*.a

# but do track lib.a, even though you're ignoring .a files above
!lib.a

# only ignore the TODO file in the current directory, not subdir/TODO
/TODO

# ignore all files in the build/ directory
build/

# ignore doc/notes.txt, but not doc/server/arch.txt
doc/*.txt

# ignore all .pdf files in the doc/ directory
doc/**/*.pdf
```

### git clone, git pull
솔직히 git clone이 폴더 만들어주는거는 까먹는다  
얘는 폴더 만든다, git init 시작, repo 받아오기, git remote 등록해준다  

clone은 다운로드, pull은 업데이트
양 측의 버전이 다르면 충돌