
https://github.com/Byunseoyoon/Github.git
# **GitHub**
markdown project 보고서

<br>

# **config**
>프로젝트를 처음 **시작**할 때, 원활하게 프로젝트 파일을 공유하고, 코드를 관리하려는 목적으로 github을 이용하기로 결정하여 각자의 컴퓨터에 git을 설치한다. 
설치 후 사용자 정보 설정을 위해 **git config**의 명령어를 사용했다. 

<br>

Git 설치 이후 첫 설정으로 **git config**명령어를 이용하여 사용자의 이름과 이메일 주소를 설정한다. ( Git을 이용하여 커밋할 때 누가 커밋했는지 지금의 정보가 남게된다. )

![config1](https://user-images.githubusercontent.com/81007682/117524598-0923f100-aff9-11eb-8e4f-bf9b5336e614.jpg)

따라서 **git config**의 명령은 사용자의 정보를 저장하고 설정을 확인하기 위해 사용될 수 있다.

<br>

`--global` 옵션은 해당 시스템에서 해당 사용자가 사용할 때는 이 정보를 사용한다. <br> 만약 프로젝트마다 다른 이름과 이메일 주소를 사용하고 싶으면 --global 옵션을 빼고 명령을 실행한다<br>
`--list` 옵션은 **git config --list** 명령을 통해 설정한 것을 확인 할 수 있다.

<br>

# **init**
> git을 설치한 이후, 프로젝트 문서를 관리할 새로운 git 저장소를 생성하기 위해서 init이라는 명령어를 사용했다.

 ![init](https://user-images.githubusercontent.com/81007682/117524600-09bc8780-aff9-11eb-97a9-0ca31b94ba45.JPG)

따라서, **git init**는 새로운 Git 저장소(repository)를 생성할 때 사용하는 할 수 있다.

<br>

# **remote**
> 각 팀원들이 git저장소를 로컬 저장소와 연결하기 위해 remote 명령어를 사용했다.

![remote](https://user-images.githubusercontent.com/81007682/117524621-0de8a500-aff9-11eb-85b2-0063f43648b4.JPG)

**remote**는 각자의 로컬 저장소에 연결하고, 저장소의 구체적인 정보들을 확인할 수 있다.

`'git remote add 이름 주소'`는 해당 이름으로 로컬 저장소에 연결을 할 수 있고, <br>
`'git remote'` 명령으로 현재 프로젝트에 등록된 리모트 저장소를 확인이 가능하며 <br>
`'git remote -v'` 옵션을 주어 단축이름과 URL을 함께 볼 수 있다.<br>
`'git remote show <리모트 저장소 이름>'` 명령으로 리모트 저장소의 구체적인 정보를 확인할 수 있다.<br>
`'git remote rename <old> <new>'`을 이용해 이름을 변경할 수도 있다.

<br>

# **clone**
> 프로젝트의 **첫번째 부분**을 담당한 팀원이 GitHub의 레파지토리에 자신의 문서를 올려 다른 담당한 팀원들이 해당 레파지토리에서 자신의 폴더에 파일을 가져오기 위하여 git clone의 명령어를 사용했다.

![clone1](https://user-images.githubusercontent.com/81007682/117524593-07f2c400-aff9-11eb-8c8b-f1d4d9521761.JPG)

해당  GitHub의 레파지스토리의 HTTPS를 복사하고, **git clone** 명령어를 이용해 자신이 원하는 폴더에 레파지스토리의 소스를 전부 복사한다. 


![clone2](https://user-images.githubusercontent.com/81007682/117524594-07f2c400-aff9-11eb-8c38-357c6e01f7d4.JPG)

<br>

Markdown project의 폴더에 GitHub의 폴더가 생성되어 Github의 레파지스토리의 소스가 전부 복사된 것을 확인 할 수 있다.

![clone3](https://user-images.githubusercontent.com/81007682/117524595-088b5a80-aff9-11eb-9be6-e3d87de38083.JPG)

이 복사된 소스를 맘대로 수정하거나 파괴해도 리모트 서버에 업로드만 하지 않는다면, 같은 리모트 서버를 보고 있는 다른 팀원이 영향을 받을 일은 절대 없기 때문에 안심하고 맘대로 만지작거려도 된다.

따라서, 해당하는 레파지토리에서 자신의 폴더에 파일을 가져오거나 복제하기 위하여 **git clone**의 명령어가 사용되는 것으로 정리할 수 있다.

`git clone -b 브랜치명 URL` 의 옵션을 이용해 특정 브랜치를 clone할 수 있다.


<br>

# **add**
> 팀원1이 올린 첫번째 작업물을 확인하고 가져온 폴더안에 피드백한 의견을 텍스트 파일로 추가한 뒤 그 파일을 git 저장소에 반영하는 과정에서 add명령어를 사용했다.

![add](https://user-images.githubusercontent.com/81007682/117524587-05906a00-aff9-11eb-94ce-0b2072d447ba.JPG)

**git add** 의 명령을 통해 Github폴더의 feedback.txt 파일을 staging area 상태에 놓았다. 따라서, 이 명령어는 파일을 staging area에 놓을 수 있게 만드는 명령어다.

+) **git add** 의 뒤에 `.` 을 입력하면 모든 파일을 staging area 상태로 만들 수도 있고, 특정한 `문서파일`을 입력하면 해당 파일만 staging area 상태로 만들 수 있다.

<br>


# **status**
> 팀원1이 초반작업하여 올린 것을 clone으로 가져온 다른 팀원이 초반 작업물을 확인하고 가져온 폴더안에 피드백한 의견을 텍스트 파일로 추가한 뒤 git 저장소에 반영하면서 git의 상태를 확인하려고 status명령어를 사용했다.

![status](https://user-images.githubusercontent.com/81007682/117524625-0e813b80-aff9-11eb-8343-7aaaa0809b1c.JPG)

**git status** 명령을 통해 feedback.txt파일이 staging area 에 놓여있지 않은것을 확인 할 수 있다.

<br>

![status2](https://user-images.githubusercontent.com/81007682/117524626-0f19d200-aff9-11eb-868d-32ec109f39dc.JPG)

git add 명령을 실행 한 뒤
다시 **git status** 명령을 하여 파일의 상태를 확인하면 feedback.txt파일이 staging area에 놓여진 것을 확인 할 수 있다. 

 **git status**명령어는 파일들의 상태를 확인 할 때 사용이 되고,  `git status -s` 또는 `git status --short` 처럼 옵션을 넣으면 현재 변경한 상태를 짤막하게 보여준다.

<br>

# **commit**
> 위에서 staging area에 놓여져 있는 feedback.txt파일을 git commit 명령어를 사용하여 수정본을 제출한다.

![commit](https://user-images.githubusercontent.com/81007682/117524597-088b5a80-aff9-11eb-953d-94e75c9078d8.JPG)

git commit의 명령어는 수정본을 제출 할 때 사용이 된다.

`git commit -m` 는 뒤에 " "안에 바로 커밋 메세지 작성할 수 있고, <br>
`git commit -a` 는 별도의 add명령어를 사용하지 않고 수정된 파일에 대해 add, commit을 한번에 수행한다. (단, 한번도 add되지 않은 파일은 add를 따로 작업 해줘야함.) <br>
`git commit -am`는 a, m의 옵션을 합친 형태이다.

<br>


# **push**
> 커밋한 feedback.txt파일을 github에 업로드 하기 위해서 push명령어를 사용하였다.

![push](https://user-images.githubusercontent.com/81007682/117524612-0b864b00-aff9-11eb-8724-46abb07f3c04.JPG)

**git push**는 원격 저장소(remote repository)에 코드 변경분을 업로드하기 위해서 사용하는 Git 명령어라고 정리할 수 있다.

`git push <저장소명> <브랜치명>`을 통해서 업로드가 가능하고, <br> 
 `-u` 옵션을 사용하면 최초에 한 번만 저장소명과 브랜치명을 입력하고 그 이후에는 모든 인자를 생략할 수 있다.<br>
`-f` 옵션은 원격 저장소 내의 해당 브랜치의 코드 변경 이력을 로컬 저장소의 코드 변경 이력으로 덮어쓴다.

<br>

# **log**
> 업로드한 feedback.txt파일을 업로드에서 지우고 직접 피드백내용을 수정해서 md 파일로 올리기로 결정하여, 파일을 지우기 위해 commit한 히스토리를 알기 위해 log 명령어를 사용했다.

![log](https://user-images.githubusercontent.com/81007682/117524603-09bc8780-aff9-11eb-9a6a-e9fb7d2daa99.JPG)

**git log** 의 명령어를 통해서 Git에는 히스토리를 조회할 수 있다.<br>
 `git log --oneline`는 히스토리를 한줄로 보여주고, <br>`git log -p` 는 각 커밋의 diff 결과를 보여준다. <br>
 `git log -2`는 최근 두 개의 결과만 보여주고, <br>
`git log --stat` 옵션은 각 커밋의 히스토리 통계 정보를 조회할 수 있다.

<br>

# **reset --hard**
>  업로드가 되어있는 feedback.txt파일을 지우고 추가 내용과 함께 직접 피드백내용을 수정해서 md 파일로 올리기로 결정하여, 파일을 지우기 위해 commit한 히스토리를 reset명령어를 사용하여 전으로 되돌아 간다.

![reset](https://user-images.githubusercontent.com/81007682/117524622-0de8a500-aff9-11eb-85a9-3d031729db5e.JPG)

**git reset --hard**의 명령어를 이용하여 커밋했던 피드백파일을 제거한다. 
<br>

따라서, reset 명령은 head를 이동시키거나 commit명령을 되돌릴 때 사용할 수 있다.
<br>

`--hard` : reset하기 전까지 했던 staging area, working directory의 작업까지 모두 reset! <br>
`--mixed(default)`: staging area은 reset, reset하기 전까지 했던 working directory의 작업은 남겨둔다. <br>
`--soft`: reset하기 전까지 했던 staging area, working directory의 작업은 남겨둔다.

<br>

> 깃헙의 레파지스토리에도 이 것을 적용하기 위해서 push를 이용한다.

![reset2](https://user-images.githubusercontent.com/81007682/117524623-0e813b80-aff9-11eb-9000-32c1d3859b99.JPG)

<br>

# **branch**
> main에 있는 첫번째 작업물이 있는 상태에서 이것을 수정하고 추가하여 만든 마크다운파일을 따로 관리하고, 이후에 병합하기 위해서 branch 명령어를 이용했다.

![branch](https://user-images.githubusercontent.com/81007682/117524590-06c19700-aff9-11eb-98d0-bd5fc1b8a2d7.JPG)

따라서, **git brach** 명령어는 코드를 수정하거나 다른 버전을 만들기 위한 목적이 있을때, 현재 가지고 있는 branch의 상태를 보거나, 새로운 branch를 추가하여 사용한다.

`-a` 옵션 : 원격 브랜치를 포함한 모든 브랜치 목록을 확인 <br>
` -m <oldbranch> <newbranch>` : 브랜치 이름변경<br>
`-d <branchname>` : 브랜치 삭제<br>
`-r` : 원격브랜치목록<br>
 `-v` : 로컬브랜치목록 + 마지막커밋내역

<br>

# **checkout**
> 위의 과정에서 feedback의 브런치가 생성된 상태에서, 이 브런치에 수정한 readme파일을 올리기 위해 checkout 명령어를 사용하였다.

![checkout](https://user-images.githubusercontent.com/81007682/117524592-075a2d80-aff9-11eb-9ec3-f9aff90c3e9f.JPG)

따라서, **git checkout**명령어는 다른 브랜치에 작업물을 올리거나 관리하려는 목적이 있을 때 현재 다른 브랜치로 전환하기위해 사용하는 것이다.

checkout 명령에 `-b` 옵션을 넣으면 브랜치 작성과 체크아웃을 한꺼번에 실행할 수 있다.

<br>

> feedback브런치를 가리키고 있는 상황에서 수정하고 추가한 readme파일을 커밋한다. 

![ch](https://user-images.githubusercontent.com/81007682/117524591-075a2d80-aff9-11eb-94ca-94f0d82d309b.JPG)

<br>

# **merge**
>  feedback브런치에 readme파일이 커밋되어있는 상태이고, 이 수정되고 추가된 feedback브런치에 있는 파일을 main에 있는 파일과 합치려고 한다. 그래서 merge라는 명령어를 사용했다.

![merge](https://user-images.githubusercontent.com/81007682/117524605-0a551e00-aff9-11eb-88ee-041421f83078.JPG)

branch를 main으로 이동해준 뒤에, git merge 의 명령을 사용해 feedback 브런치와 결합하였다.

**git merge**라는 명령어는 나눠져있는 브런치를 결합하기 위해서 사용하는 것으로 정리할 수 있다.

`git merge --abort` : Merge 하기 전으로 되돌린다.<br>
`git merge --squash` : 현재 브랜치에 병합 대상과 차이나는 commit을 하나로 합쳐서 커밋한다.

<br>

> feedback브런치를 main에 병합한 상태를 github의 레파지스토리 업로드 하기 위해서 push명령어를 사용해 준다.

![mp](https://user-images.githubusercontent.com/81007682/117524606-0a551e00-aff9-11eb-9d97-7e66491dd7be.JPG)

<br>

> 병합한 상태의 README 파일의 이름을 Markdown으로 바꾸기 위해서, 파일 이름을 바꾸고 add와 commit을 해준다. 

![mp2](https://user-images.githubusercontent.com/81007682/117524607-0aedb480-aff9-11eb-988f-bede00a53369.JPG)

<br>

# **pull**
> 수정되고 추가된 파일이 병합되고 깃헙이 갱신 되어있는 상태에서 다른 팀원들이 갱신된 파일을 확인하려는 목적으로 각자의 폴더에 내려받기 위해 pull이라는 명령어를 사용했다.

![pull](https://user-images.githubusercontent.com/81007682/117524611-0b864b00-aff9-11eb-8a1f-7715adbe7748.JPG)

이 명령어를 이용해 자신의 폴더에 최신코드를 가져왔다.

따라서, **git pull** 명령어는 협업과정에서 갱신된 레파지스토리의 최신 코드와 문서들을 로컬 레파지스토리에 가져오는 역할로 사용되는 것으로 정리할 수 있다.

`git pull --rebase 저장소 브랜치명` : 명령어를 실행할 때 merge가 아닌 rebase 방식으로 병합할때 사용할 수 있다.

<br>

> 갱신된 파일을 가져와 md 파일을 확인한 다음 더 이상 수정사항이나 변경사항이 없는 상태에서, 이 md파일과 여기서 사용되는 사진들을 zip파일로 합쳐서 레파지스토리에 올리려고 할 때, 앞에서 사용한 명령어인 add, commit, push를 사용하여 zip파일을 레파지스토리에 적용한다.

![pu](https://user-images.githubusercontent.com/81007682/117524610-0aedb480-aff9-11eb-8224-cf2672fe6efa.JPG)

<br>

# **tag**
> zip파일을 레파지스토리에 적용한 이후 head가 zip파일의 커밋을 가리키고 있는 상태에서, 이 파일이 최종 버전이라고 태그를 달기 위해서 tag 명령어를 사용하였다.

![tag](https://user-images.githubusercontent.com/81007682/117524627-0fb26880-aff9-11eb-98bb-9dfdcca79889.JPG)

**git tag**는 저장소의 소스 버전을 간간히 표시하기 위해서는 커밋 메시지 또는 브랜치로 해서 표시하는 것 보단 태그로 깔끔하게 할 때 사용하는 것으로 정리할 수 있다.

`git tag` : 태그를 조회할 때 사용할 수 있다.<br>
`git tag [Tag Name]` : Lightweight 태그는 특정 커밋을 가르키는 역할로 Lightweight 태그를 붙일 수 있다.<br>
`-a` 옵션을 붙여 태그를 만든 사람, 이메일, 날짜, 메시지를 저장할 수 있다.<br>
`-l` 옵션을 붙여 원하는 태그명의 조건을 붙여 검색이 가능하다.

<br>

# **rebase**
> 팀원들이 갱신된 파일을 확인을 해 본 후, 더이상 수정할 부분이 없다고 생각하여 올라와 있는 Markdown파일의 "name change"라고 메세지를  메세지를 "final md file" 라고 수정하기 위해서 rebase의 명령어를 사용했다.

![rebase0](https://user-images.githubusercontent.com/81007682/117524614-0cb77800-aff9-11eb-810f-ccfef8458d6c.JPG)

git log를 사용하여 알아낸 commit값을 **git rebase -i 값**에 넣어서 명령을 실행한다.

<br>

![rebase](https://user-images.githubusercontent.com/81007682/117524613-0c1ee180-aff9-11eb-9da0-44f93953a34f.JPG)
나와있는 명령어들 중에서 커밋의 메세지만 바꾸는 명령어를 확인하고 바꿀 커밋 앞의 'pick'을 'reword'로 저장해준다.

<br>

![rebase3](https://user-images.githubusercontent.com/81007682/117524618-0d500e80-aff9-11eb-9ac1-689c156bdb2b.JPG)

그리고 name change라고 나와있는 메세지를 final md file로 변경시킨뒤 저장을 해준다.

<br>

![rebase4](https://user-images.githubusercontent.com/81007682/117524619-0d500e80-aff9-11eb-8b68-0eba17a8a8be.JPG)

git log명령어를 통해 commit의 메세지가 바뀐 것을 확인 할 수 있고, git push명령어를 통하여 리모트 버전에 갱신을 해주었다.

**git rebase** 명령어는 커밋을 수정하거나 바꾸고 싶은 부분이 있을 때 나와있는 다양한 edit 명령어를 입력하여 사용하는 것으로 정리할 수 있다.

`git rebase [newbase]`이 명령어를 사용하면 한 브랜치에서 다른 브랜치로 합치는 방법을 Merge대신 Rebase로 사용할 수 도 있다.<br>
`git rebase -i $[수정할 커밋의 직전 커밋]` 수정할 직전의 커밋은 '커밋의 해시'를 이용하거나 'HEAD~3'처럼 HEAD를 기준으로 작성이 가능하다. 이 옵션을 사용하게 되면 여러가지 edit 기능이 있는 vim이 나오게 되어 다양한 edit 기능을 선택하여 사용할 수 있다.<br>
`git rebase --onto branch1 branch2 branch3` 이 옵션은 branch1 브랜치부터 branch2 와 branch3의 공통 조상까지의 커밋을 branch3 브랜치에서 없애고 싶을 때 사용한다.


<br>

<br>

|종류|사용여부|URL|
|:--:|:--:|:--|
|add|O|https://github.com/Byunseoyoon/Github#add|
|branch|O|https://github.com/Byunseoyoon/Github#branch|
|checkout|O|https://github.com/Byunseoyoon/Github#checkout|
|clone|O|https://github.com/Byunseoyoon/Github#clone|
|commit|O|https://github.com/Byunseoyoon/Github#commit|
|config|O|https://github.com/Byunseoyoon/Github#config|
|init|O|https://github.com/Byunseoyoon/Github#init|
|log|O|https://github.com/Byunseoyoon/Github#log|
|merge|O|https://github.com/Byunseoyoon/Github#merge|
|pull|O|https://github.com/Byunseoyoon/Github#pull|
|push|O|https://github.com/Byunseoyoon/Github#push|
|rebase|O|https://github.com/Byunseoyoon/Github#rebase|
|remote|O|https://github.com/Byunseoyoon/Github#remote|
|reset --hard|O|https://github.com/Byunseoyoon/Github#reset---hard|
|status|O|https://github.com/Byunseoyoon/Github#status
|tag|O|https://github.com/Byunseoyoon/Github#tag|
