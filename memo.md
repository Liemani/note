### To Do (구체적이면 좋습니다.)

- search keyword
  - architecture
  - underneath
  - underlying mental model and architectur
- env
  - base camp 를 짓는 것 처럼 env 폴더가 존재하는 위치를 중심으로 programming 폴더를 만든다면 더 좋을 것 같다
  - preparetheday, finishtheday 를 backup, backdown 으로 해도 괜찮을 것 같다
  - backup 시 commit message 를 back up 이라고 해도 좋을 것 같다
  - aux
    - vimcommand gitlog 처럼 alias 변수를 특정 shell 파일로 실행하는 경우 zsh 로 실행하게 되면 해당 shell script 가 alias 변수를 알지 못한다
  - 모듈화시키기 위해 전역변수를 쓰지 않도록 만들었는데 이로 인해 전역에 있는 alias 를 인식하지 못하는 문제가 발생한다
    - 즈 alias 를 인자 등으로 전달하기 위해서는 $(whence command) 등으로 전달하도록 하자
- git
  - 커밋을 삭제하는 방법?
  - how to colaborate with another user in github.com private repository?
  - pull request 는 어떻게 돌아가는 것일까?
  - 모든 git 관련 데이터는 사라지지 않는다고 했는데
    - 그럼 브랜치를 삭제해도 해당 브랜치에서 커밋한 내용들도 다 살아있는 것일까? 살아있다면 어떻게 출력해볼 수 있을까?
	- 모든 commit 을 graph 로 출력할 수 있었으면 좋겠다
  - 원격 저장소에 있는 다른 branch 를 삭제하는 방법도 있을까?
  - merge 는 특정 commit 까지를 병합하는 것으로 알고 있는데 혹시 특정 commit 만 merge 하는 방법도 있을까?
  - 그런대 너무 branch 를 산발적으로 만들면 branch 를 탐색하기 위한 commit 적용 시간이 나중엔 너무 길어지는 것이 아닐까?
    - 그냥 어느정도는 git 하나에 몰아넣는 것 보다 쪼개는 것이 좋지 않을까?
	- swift 의 git 크기는 약 624 MB 로, 다양한 commit 으로 이동할 때 시간이 많이 걸리지 않을까?
      - 시간이 많이 걸리지는 않았다
  - git workflow
    - git flow
	- cherry pick?

- git
  - 생활코딩/GIT4 보기
  - 여러 커밋의 diff 를 하나처럼 출력하는 방법?
- get\_next\_line
  - dummy node 를 만들 때 장점?
  - BUFFER\_SIZE 크기의 버퍼에 데이터를 line 에 복사하는 와중에 메모리 할당 에러가 발생하면 얼마나 정리하고 프로그램을 종료시켜야하나?
  - eof 를 만났을 때 해당 버퍼를 free 해줘야 하는가? 안해줬는데
  - test
    - test program
      - gnl-war-machine-v2019
	  - 42cursus\_gnl\_tests
	  - gnlkiller
	  - gnlTester
    - memory leak test
    - 다양한 입력값에 대해 테스트하기
    - 다양한 BUFFER\_SIZE 테스트
    - pdf 의 노란 박스 테스트하기
    - wiki.42seoul 의 에러 관리 점검하기
- netwhat
  - 디펜스하기

- didplay memory
  - add, move, remove 명령어로 메모리의 오른쪽에서 특정 주소를 가리키는 포인터 그래픽을 조작할 수 있는 기능 추가
- printf

- 맥 공유 기능 알아보기
- 읽고 싶은 책
  - cs
  - modern c
  - The C Programming language
- 이사 일정 생각해보기
  - 이사는 최소 1 월달 돈이 들어오고 나서이다
  - 그리고 시험이 원활이 돌아가고 클러스터가 개장하면 서울에 가서 공부를 하는 것이 좋다
  - 평가도 직접 대면해서 진행하면 더 수월할 것이다
  - 즉 서울로 이사가는데 영향을 미치는 요소는 클러스터 오픈, 원활한 시험 진행
- git
  - commit 관리하는 방법
    - 이동, 이동하며 커밋, 과거 기록 변경 등
  - 생활코딩 git 보기 ㅎㅎ
  - [Git Tips](https://github.com/mingrammer/git-tips)
- mac-air11
  - 윈도우에 ddns 서버 실행시키기
- display\_memory 에 2, 3, 4 번째 인자를 통해 prev, cur, end 를 표현하도록 하기
  - add, remove, move 등의 명령어를 통해 포인터 그래픽을 움직일 수 있으면 좋겠다 ㅎㅎㅎㅎ
- get\_next\_line
  - apply free list function when error occured
  - shoul EOF when end whith '\n'?

### memo

#### 2021-01-28

클러스터는 예약시스템 지금은 코로나가 심해져서 예약조차 안되는 듯 하다
2.5 단계 밑으로 내려가야 클러스터 사용이 가능하다

#### 2021-01-15

```zsh
% cat display_line.sh
$1 | wc -l
% ./display_line.sh set
      41
% sh display_line.sh set
      41
% zsh display_line.sh set
     145
% set | wc -l
     167
% source display_line.sh set
     167
% bash

The default interactive shell is now zsh.
To update your account to use zsh, please run `chsh -s /bin/zsh`.
For more details, please visit https://support.apple.com/kb/HT208050.
bash-3.2$ set | wc -l
      47
```

- 왜 set 의 결과 값이 달라지는 것일까?

#### 2021-01-14

- 전선이 모든 주파수를 다 통과시키지 못하고 제한된 영역의 주파수만 전달이 가능한 이유가 무엇일까? [youtube](https://youtu.be/1pfTxp25MA8?t=368)
- 디지털 신호도 원하는 주파수를 만들어서 전송할 수 있을 것 같은데 굳이 아날로그 신호로 바꾸어서 전송해야 하는 이유가 무엇일까? [youtube](https://youtu.be/1pfTxp25MA8?t=386)

### time line

2020-10-13

ctrl a
ctrl e

opt <-
opt ->

ctrl u
ctrl k

hexdump

Put some unfamiliar shortcut image aside. 


2020-11-17
POSIX CLI1
https://opentutorials.org/module/3747


2020-11-27
which vimmemo
(in vim normal mode): ":echo $MYVIMRC"
	# You can easily find the location and name of the file on any operating system.
how to move cursor to top or bottom of screen in vim?
	# H: move cursor to top of screen.
	# L: move cursor to bottom of screen.
	# {: move cursor to previous paragraph.
	# }: move cursor to next paragraph.
why use link?
	# For to call same function as different names
what is the difference between soft link and hard link?


# 2020-12-08

1.3. x: delete a character
1.4. i: enter `insert mode`
1.5. a: enter `insert mode` with appending

2.1. dw: delete a word
2.2. d$: delete to the end of line
2.3. `command target`: dw, de, d$
	enable target example: w, e, $, 0, b, h, j, k, l, H, L, {, }
2.4. `count command`: 2w, 3e
	0: move cusor  the start of the line
2.5. `command count target`: d2w
2.6. dd: delete a line
	`count command target`: 2dd, 2dw
2.7. u: undo last command
	ctrl-r: redo last undo

3.1. p: put vim's buffer content behind the cursor
	if vim's buffer has a line, put it under line of the cursor
3.2. r: replace a character without mode change
3.3. c target: delete target and enther `insert mode`(change): ce, c$, c2w, 2cw

4.1. ctrl-g: display the path of the file and state
	G: move to the last line of the file
	gg: move to the first line of the file
	count G: move to the count line
4.2. / 'what to search': search downward
	? 'what to search': search upward
	n: search next
	N: search previous
	ctrl-o: move previous cursor position
	ctrl-i: move next cursor position
4.3. %: move to the matching bracket
4.4. :s/old/new/g: subtitute 'old' to 'new'
	:s/thee/the: subtitute only first encountered 'thee'
	:s/thee/the/g: subtitute all(globally) 'thee' to 'the' in this line
	:#,#s/old/new/g: #,# mean the line number of two line
	:%s/old/new/g: search target from whole the file
	:%s/old/new/gc: you can command by prompt whether subtitute or not

5.1. :! 'extern command' <ENTER>: excute extern command
5.2. :w FILENAME: write current file as FILENAME
5.3. :\'\<,\'\>w FILENAME: save selected range as FILENAME
5.4. :r FILENAME: read and put FILENAME file under the cursor line
	:r !ls: read and put the result of 'ls' extern command under the cursor line

how to show pressed command state?
default output resolution: 853x480


2020-12-23
- Q: I can set the data type of function as array or pointer, if I set the type as array, will it take all feature of array? (or it's actually just pointer)
    char    str[] = "lol";
- Q: imo, `"lol"` might be stored in data block and copy it to str array, correct?


2020-12-24
(Q: Question, I: Idea)
- Q: When i set the argument type of main, even making it pointer is common, making it array also possible, will there some difference?
- Q: Will it possible executing according to the extension of file in vim?
  - :set autoindent for .md
  - :set cindent for .c
- I: What about a program which show real memory state on one side and what happenning at code at the other side?
  - Simulate very little computer, so i can see the memory at one display
- Q: Can i access NULL pointer?
- Idea: mobile golf game
  - Scroll the mobile display, if your display stop at to goal, you are hole in one :D


2020-12-25
(T: Think, D: Do)
- T: Ratio of my study and others study
  - Just help others study, and if i get some thought of 'It's not right', then reject it
  - Never present a fish, teach how to get that
- D: More practice the way to use `find` command


2020-12-26
- ft\_memcpy: 14:07 ~ 14:13
- ft\_memccpy: 15:09 ~ 15:50


2020-12-27
- ft\_memmove: 11:07 ~ 11:22
- ft\_memchr : 11:22 ~ 12:00
- 13:30 ~ 18:00


2020-12-28
- 14:00 ~ 
- memchr: 16:05 ~
- memcmp: 16:25 ~ 16:47
- strlen: 16:48 ~ 17:09
- strlcpy: 17:12 ~


2020-12-29
- 10:30 ~
- strlcat: 10:38 ~ 12:03 - 10
- ~ 12:14
- 13:46 ~
- strchr: 13:47 ~ 14:02
- strrchr: 14:04 ~ 14:25, 14:27
- strnstr: 15:01 ~ 16:00
  - 16:05 - 5 ~ 16:37	
  - 16:41 ~ 16:48
- strncmp: 
  - 16:55? ~
  - 17:06 ~ 17:10
  - 17:22
- atoi:
  - 17:28 ~ 18:03
  - 18:03 ~ 18:47
- ~ 20:30

white space characters:
'\t', '\n', '\v', '\f', '\r', ' '


2020-12-30
- segmentation fault shoul occure at appropriate time.. let me modify...
- 09:43 ~ 12:14
- 13:25 ~ 13:56
- 14:20 ~ 18:00
- 21:10 ~
- isalpha
  - 21:11 ~ 21:28
  - 21:31 ~ 21:35
- isdigit
  - 21:37 ~ 21:47
  check something cmp
- ~ 22:15


2020-12-31
- isalnum
  - 09:39 ~
  - 09:46 ~ 09:48
- isascii
  - 09:53 ~
  - 09:59 ~ 10:01
- isprint
  - 11:34 ~
  - 11:45 ~
- ~ 11:55
- 13:49 ~
- toupper
  - 13:50 ~
  - 14:10 ~
- ~ 14:17
? 그럼 a 인데 int 범위에 값이 있어도 참인가?
- tolower
  - 16:59 ~ 
  - 17:17 ~
- calloc
  - 17:20 ~ 
  - 18:25 ~ 18:28
- ~18:33


2021-01-01
- 11:00 ~
- strdup
  - 11:51 ~ 11:55
  - calloc
    - ~ 12:04
  - ~
  - 12:11 ~ 12:20
- ft\_substr
  1. 12:46 ~
  2. 13:30 ~
  3. 13:47 ~
  4. 14:05 ~
  5. 14:20 ~
  6. 14:51 ~ 15:05
- ft\_strjoin
  1. 15:08 ~
  2. 16:16 ~ 16:50
- ft\_strtrim
  1. 20:13 ~
  2. 20:30 ~ 20:55
  3. ~ 21:07
- ft\_split
  1. 21:10
  2. 21:14 ~ 21:54


2021-01-02
- 12:20 ~
- ft\_split
  1. 12:29
- ~ 13:23
  1. 13:30 ~ 16:19
- ft\_itoa
  1. 16:35 ~
  - -5
  2. ~ 17:38
- ~ 17:45
- 19:17
  - ~ 20:55
  - 21:02 ~ 21:14
  - 21:17 ~ 21:19
  - 21:21 ~ 21:25
  - 21:26 ~
  - -5
  - ~ 21:56


2021-01-03
- 10:36
- ft\_lstnew
  - 11:07 ~ 11:17
- ft\_lstadd\_front
  - 11:24 ~ 11:36
- ft\_lstsize
  - 11:40 ~ 11:58
  - 12:02 ~ 12:05
- ft\_lstadd\_back
  - 12:10 ~ 12:17
- ft\_lstdelone
  - 12:37 ~ 12:41
- ft\_lstclear
  - 12:42 ~ 12:55
- ft\_lstiter
  - 12:57 ~ 13:01
- ft\_lstmap
  - 13:11 ~ 13:25
- 16:36 ~
  - ~ 17:06
- ~ 18:00
- 19:22 ~
- memmove
  - 20:39 ~ 20:51
- ~ 21:34


2021-01-04
- 06:19 ~ 11:30
- 17:34 ~ 19:22
- 21:00 ~ 21:52


2021-01-05
- 09:27 ~ 11:33
- ~11:53
- 13:00 ~
  - netwhat
  - 13:27 ~ 14:05
  - 14:40 ~ 18:30
- 20:14 ~ 21:41


2021-01-06
- 08:05 ~ - 5 ~ 09:00
- 10:54 ~ 11:51
- 13:26 ~ - 15 - 40 - 10 ~ 19:10
- 20:57


2021-01-07
- 09:00 ~ 11:00
- 20:00 ~ 22:26


2021-01-08
- 10:10 ~ 12:00
- 15:56 ~ 16:51 ~ 18:21


2021-01-11
- 09:30 ~ 11:20


2021-01-13
- vim 에서 alias 로 설정한 명령을 부를 수 있을까?
