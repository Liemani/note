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
5.3. :'<,'>w FILENAME: save selected range as FILENAME
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
