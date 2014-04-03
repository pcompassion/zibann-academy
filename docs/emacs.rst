============================
 사용하는 emacs key binding
============================


cursor movement
===============


+----------------------------------------+----------------------------------------+
|위로                                    |C-p                                     |
+----------------------------------------+----------------------------------------+
|아래로                                  |C-n                                     |
+----------------------------------------+----------------------------------------+
|한단어 앞으로                           |M-f                                     |
+----------------------------------------+----------------------------------------+
|한단어 뒤로                             |M-b                                     |
+----------------------------------------+----------------------------------------+
|한글자 앞으로                           |C-f                                     |
+----------------------------------------+----------------------------------------+
|한글자 뒤로                             |C-b                                     |
+----------------------------------------+----------------------------------------+
|한줄 맨 앞으로                          |C-a                                     |
+----------------------------------------+----------------------------------------+
|한줄 맨 뒤로                            |C-e                                     |
+----------------------------------------+----------------------------------------+
|버퍼 맨 앞으로                          |M-<                                     |
+----------------------------------------+----------------------------------------+
|버퍼 맨 뒤로                            |M->                                     |
+----------------------------------------+----------------------------------------+

+----------------------------------------+----------------------------------------+
|한단어를 앞으로 지우기                  |M-d                                     |
+----------------------------------------+----------------------------------------+
|한단어를 뒤로 지우기                    |M-backspace                             |
+----------------------------------------+----------------------------------------+


copy and paste
==============

C-space 로 시작점을 잡고, 위의 방법으로 커서를 이동하여 원하는 영역을 선택한다
잘라낸 영역은 차례대로 기억되며, 이전에 잘라놓은 것들도 사용할 수 있다.

+----------------------------------------+----------------------------------------+
|copy                                    |M-w                                     |
+----------------------------------------+----------------------------------------+
|잘라내기                                |C-w                                     |
+----------------------------------------+----------------------------------------+
|붙여넣기                                |C-y                                     |
+----------------------------------------+----------------------------------------+
|이전 내용 붙여넣기                      |M-y                                     |
+----------------------------------------+----------------------------------------+


검색
====

+----------------------------------------+----------------------------------------+
|파일 찾기                               |C-x M-p                                 |
+----------------------------------------+----------------------------------------+
|단어 찾기                               |C-c g                                   |
+----------------------------------------+----------------------------------------+
|현재 커서가 있는 단어 찾기              |C-c k                                   |
+----------------------------------------+----------------------------------------+
|열려진 버퍼를 이름으로 찾기 (단어 사이에|C-x b                                   |
|C-space 를 입력해서 결과를 좁힐 수 있다)|                                        |
+----------------------------------------+----------------------------------------+
|현재 커서 뒤에 있는 단어 찾기           |C-s                                     |
+----------------------------------------+----------------------------------------+
|현재 커서 앞에 있는 단어 찾기           |C-r                                     |
+----------------------------------------+----------------------------------------+


버퍼
====

+----------------------------------------+----------------------------------------+
|이전 버퍼                               |C-x <-                                  |
+----------------------------------------+----------------------------------------+
|다음 버퍼                               |C-x ->                                  |
+----------------------------------------+----------------------------------------+

window
======

+----------------------------------------+----------------------------------------+
|윈도우를 상하로 나누기                  |C-x 3                                   |
+----------------------------------------+----------------------------------------+
|현재 윈도우를 없애기                    |C-x 0                                   |
+----------------------------------------+----------------------------------------+
|다음 윈도우로 이동하기                  |C-x o                                   |
+----------------------------------------+----------------------------------------+
|현재 윈도우만 남기기                    |C-x 1                                   |
+----------------------------------------+----------------------------------------+


find and replace
================

+----------------------------------------+----------------------------------------+
|현재 커서로부터 검색                    |M-%                                     |
+----------------------------------------+----------------------------------------+
|여러 파일 내용을 한꺼번에 수정-1        |M-x find-grep-dired 로 먼저 검색하고, m |
|                                        |과 t 로 마킹한뒤 Q 를 누른다            |
+----------------------------------------+----------------------------------------+
|여러 파일 내용을 한꺼번에 수정-2        |C-c g 로 검색한 결과를 C-x C-s 로       |
|                                        |저장한후 M-n M-p 로 파일을 이동하면서   |
|                                        |M-% 를 실행한다                         |
+----------------------------------------+----------------------------------------+


indent
======

+----------------------------------------+----------------------------------------+
|indent 할 영역에 대하여                 |M-;                                     |
+----------------------------------------+----------------------------------------+
|web-mode 에서는                         |C-c tab                                 |
+----------------------------------------+----------------------------------------+