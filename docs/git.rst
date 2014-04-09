==============
 git tutorial
==============


git 이 뭐냐
===========

source (주로 텍스트 파일) 을 수정한 것에 대한 기록
기록한 곳으로 돌아가기
기록한 곳들의 차이점을 보기


git tip 들
==========

- directory (log 디렉토리 라고 하자) 는 git 에 넣고 싶은데, 그 안의 파일들은 git 에 넣고 싶지 않다.

  ::
	 *
	 !.gitignore

  위 내용의 .gitignore 파일을 만들어 log 디렉토리에 넣는다.
  log 디렉토리내에서 .gitignore 파일을 제외한 다른 모든 파일을 무시한다.

  http://stackoverflow.com/a/5581995/433570

  
