### To Do (구체적이면 좋습니다.)

#### 개인

- 기록이 먼저
  - 작성한 report 를 github.io 에 업로드하기
  - 내가 프로그램 지능이 나보다 낮은 사람에게 알려줄 수 있는 것은 앞길과, 그 시기에는 원래 그렇게 힘들다는 것이다
  - 프로그래밍 단어 정규화
  - record 가 push 까지 하면 실시간으로 백업이 가능하다
  - 자동으로 웹에 백업되는 것도 좋지만, 시간이 오래 걸리는 작업이기 때문에 캐쉬를 기본으로 하고 필요에 따라 사용자에게 백업 및 풀 권한을 주는 것도 좋을 것 같다
  - 태그가 github 에 push 되지 않았다. 어떻게 올리는지 알아보자
  - libft 같은 경우 hard link 로 만들어도 좋은걸까?
  - link file 은 깃허브에 어떻게 올라갈까? (아니면 깃에 어떻게 기록될까?)
	- 깃에도 똑같이 링크 파일로 기록될 것 같다
	- 깃이 권한이나 등등 메타 데이터도 기록할까?
  - 생각
    - 프로그램의 구조를 다 보여주는 프로그램은 어떨까?
	  - lldb 처럼 디버깅용 프로그램인데 어떤 함수에 어떤 변수가 존재하는지 다 보여주고 어떤 변수가 어떤 변화과정을 겪었는지 연대기를 다 보여주는거지
    - 많이 생각해보면 좋을 것
      - null guard 의 형식 등 통일된 형식을 만들고 지키는 문제
    - 생각을 적게 해야할 부분
	  - 여러 이름들, 최선의 이름은 있겠지만 최고의 이름은 없다
  - how to multi line quote in md
  - == 연산자는 어떻게 0 과 1 을 반환하는가?
  - 인자가 특정 값이면 0 을 반환하는 함수?
  - ls 에 파일 내용을 출력하는 기능이 있더라
  - git log --branches 가 remote branch 는 보여주지 않는 문제
  - env 가 setenv.sh 를 실행할 때 설정해줘야하는 파일을 vim 으로 열어도 좋을 것 같다
  - va\_list 인자는 기존 인자와는 다른 방식으로 작동하는 모습을 보이는 것 같다. 더 큰 크기의 인자로 받아들일 때도 입력받은 인자의 크기만큼을 가져온다. 내부적으로 어떻게 되어있는 것일까?
  - 기록 관리 프로그램 in cli!!!!
    - git 처럼 vcs 이 아니라 기록 control system 을 만들자!
	- git 에 자료를 보관하면서 보관되어 있는 자료를 쉽게 control 하는거지!
  - 블로그에 날짜 표시하기
  - 함수 이름을 여러개로 쓸 수 있도록 필요할 때마다 추가할 수 있도록 하면 결국 지저분해질 뿐이다, 따라서 문서 편집기에서 특정 이름들을 특정 상수로 바꾸도록 처리하여 서로 다른 이름을 쓰더라도 결국 같은 상수가 되도록 처리하는 것이 좋다. 일괄적으로 변수 이름을 바꾸는 기능을 상위단에서 제공하는 것이다
  - 모든 local repo 의 branch 를 출력하는 프로그램은 어떨까?
  - 문서편집기인데 모든 문자들이 저마다의 태그를 가지고 있고 특정 태그의 특정 문자나 단어를 replace 할 수 있는 프로그램
  - :set all: display all set
  - 데이터를 마구마구 던지면 알아서 구조화하고 정리해주는 프로그램
  - 일단 명령을 입력하기가 무조건 쉬워야 한다 (혹은 alias 를 사용할 수도 있겠지), 그러고 나서 보기 좋게 출력하는 것은 추가적인 출력 프로그램이 담당하는 것!
  - dummy node 의 장단점
- 정리하기
  - 북마크
  - 읽기 목록
  - 하드
  - 메모
  - 슬랙 saved
- search keyword
  - architecture
  - underneath
  - underlying mental model and architectur
- env
  - base camp 를 짓는 것처럼 env 폴더가 존재하는 위치를 중심으로 programming 폴더를 만든다면 더 좋을 것 같다
    - 이 경우 vim 에서는 절대 경로를 사용하는데 어떻게 처리해줘야하는 것일까?
	  - 상대경로를 통해 생성한 절대결로로 해당 절대 경로 데이터를 바꿔줘야만 할까? 너무 복잡한데?
  - back command 가 인자를 받아서 해당 git repo 만 처리하도록 하자
- git
  - how to get the content of hash?
  - [Git Tips](https://github.com/mingrammer/git-tips)
- lldb
  - 특정 시그널 보내기
  - 'memory read': 메모리를 출력함
- 책
  - 50/288 : The C Programming Language
  - 늑향: 10 권 114p
- variabledText
  - 변수의 값에 '\n' 를 넣을 수 있게하려면 변수 간의 delimiter 를 '\n' 로 하면 안되는 걸까?
  - 변수 식별자를 일괄적으로 바꾸는 추가 기능
  - 다양한 경고 (위치와 해당 라인 출력)
    - 정의하지 않은 식별자 사용 경고
    - 사용하지 않은 식별자 정의 경고
    - 중복 정의된 식별자 경고
  - 프로그램 실행을 global 하게 설정하는 방법



#### 보고서

- miniRT
  - mandatory
    - 5 geometric objects: plane, sphere, cylinder, square, triangle
	- 겹치는 경우와 오브젝트 내부도 올바르게 처리되야 한다
	- 오브젝트의 속성을 resize 할 수 있어야 한다
	- 평행 변환과 회전 변환이 가능해야 한다
	- 빛
	- 두 번째 인자로 '--save' 를 받을 경우 이미지를 bmp 형식으로 저장하기
	- 만약 두 번째 인자가 주어지지 않았다면 아래와 같은 기능 수행하기
	  - <ESC> 가 창을 닫고 프로그램을 깔끔하게 종료해야 한다
	  - 창의 붉은 종료 버튼을 클릭하면 창을 닫고 프로그램을 종료해야 한다
	  - 요구된 scene 크기가 화면보다 크다면 창 크기를 화면 해상도에 맞게 설정하기
	  - 만약 카메라가 여러개 존재한다면 원하는 키를 눌러서 화면 전환이 가능하도록 하기
	- 첫 인자는 .rt 확장자를 갖는 scene description 파일을 입력받는다
	  - .rt 파일이 잘못 구성되어 있다면 "Error\n" 를 출력하며 프로그램 종료하기
  - 라이브러리의 경우 <> 로 include 가 가능하게 되는 것일까?
  - rasterization 검색
  - api 사용해보기
  - 이미지 출력 전에 client 의 endianess 를 확인한 후 server 의 endianess 에 따라 이미지 처리하기
- ft\_server
  - Nginx 알아보기
  - 슬랙, 디코, 42wiki 에서 정보 얻기
  - vnc 로 돌려보기
  - Wordpress
  - phpMyAdmin
  - SQL databse
- exam02 준비
- 블로그를 어느정도 자동화 시켜주는 툴 만들기

#### 미래

- 42 seoul 언급 외의 공부해온 내용을 정리하여 블로그에 올리기
  - 하지만 그것을 위해서는 먼저 블로그가 잘 정돈되어야 할 것이다
  - makefile
  - lldb
  - vim
  - git
  - git log pretty format
  - cli
  - shell script
  - free 후 참조 -> 바로 사용해도 잘못된 값이 들어갈 수 있음 (확률)
    - malloc 의 크기이면 malloc 에러
	- free 면 segmant fault
	- 참조면 abort 나 bus error
- 사이드 프로젝트
  - 게임을 만들고 싶은데 (아니면 간단한 보조 프로그램이라도) 혼자 하는건 싫고 반드시 멀티가 가능하도록 만들고 싶다!!!!!!!
    - 개인 플레이 게임을 만드는 것도 크게 나쁘지는 않으나 재미를 얻을 수 있는 요소가 멀티에 비해 제한된다
- 읽고 싶은 책
  - Computer Organization and Design: 많은 대학에서 사용하는 컴퓨터 구조의 바이블
  - 성공과 실패를 결정하는 1%의 네트워크 원리
  - strunk and white
  - Real-World Software Developement
  - code (?)
  - cs
  - [modern c](https://modernc.gforge.inria.fr)
  - The C Programming language
  - https://git-scm.com/book/en/v2
  - Don't Make Me Think
  - [Laws of UX](https://lawsofux.com/)
  - Code Complete
  - Writing Solid Code
- 이사 일정 생각해보기
  - 냉장고는 있어야 한다
  - 화장실이 있는 것도 큰 메리트이다 (화장실을 다른 사람이 다 쓸 때까지 기다리지 않아도 된다)
  - 빗자루, 걸래 정도의 청소도구는 있는 것이 좋다
  - 평가도 직접 대면해서 진행하면 더 수월할 것이다
  - 아침에 뛰기 위해 러닝복, 러닝화도 가져가도록 하자
  - 속옷은 총 4 벌, 양말은 5 짝 외출복은 2 ~ 3 벌, 외투는 아주 두꺼운거 1 개 평범한거 1 개
  - 마스크
  - 휴지, 밥그릇 (유리 재질 2 개면 좋다), 세면 용품, 이불
- mac-air11
  - 윈도우에 ddns 서버 실행시키기
    - 실행해도 지금 가지고 있는 공유기가 DNS client 를 가지고 있지 않는 듯 해서 의미가 없다..
- display\_memory 에 2, 3, 4 번째 인자를 통해 prev, cur, end 를 표현하도록 하기
  - add, remove, move 등의 명령어를 통해 포인터 그래픽을 움직일 수 있으면 좋겠다 ㅎㅎㅎㅎ

### memo

#### 2021-04-11

- 다음 두 함수의 차이가 있을까?

```c
int strlen(char s[])
{
	int	i;

	i = 0;
	while (s[i] != '\0')
		++i;
	return i;
}
```

```
int	strlen(char *s)
{
	char	*ptr;

	ptr = s;
	while (*ptr)
		++ptr;
	return (ptr - s);
}
```

- -1L vs 1UL: unsigned long 타입으로 변환되고 비교한다면 -1L 이 더 크게 된다. 실제는 어떨까?

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

2020-??-??

echo "*"    # *
echo '*'    # *
echo /*    # *
echo *    # display all files
echo ~    # display home path
echo ?    # display all 1 character

echo "$truc"    # isACar
echo '$truc'    # truc

cat [-e]
more    # work like man page
head
tail

grep [-iv]

ls bonjour 2> error.log
ls bonjour test* > res.txt 2> error.log
ls bonjour test* 2> error.log | grep test00

cat batman.txt | grep Joker | wc -l
grep Joker < batman.txt | wc -l

echo coucou > res.txt    # write file
echo coucou >> res.txt    # append file

cat << FIN    # read until FIN
ls bonjour *.txt > resultat.txt 2>&1
cat resultat.txt

ctrl d
ctrl c
ctrl \

2020-10-14
gzip -d <file>
tar -zxvf <file>
man cut
man diff
man patch

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
