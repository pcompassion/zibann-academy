
reStructuredText Tutorial
=========================


reStructuredText 를 쓰는 이유
-----------------------------

좋단다.. 쉽게 배워서, 쉽게 작성해서 문서를 만들수 있다.
ReadTheDocs 에 올리려니, 이걸 써야 된다. (또는 markdown)


.. __simple-exampl-label:

간단한 예제
-----------

헤더::

  Section Header
  ==============

  Subsection Header
  =================


Lists::

  - 나는 잘생겼고
  - 배도 나왔고
  - 애도 잘 키워
	1) 지안이도
	2) 정우도

Link::

  A sentence with links to Wikipedia_ and the `Linux kernel archive`_.

  .. _Wikipedia: http://www.wikipedia.org/
  .. _Linux kernel archive: http://www.kernel.org/
  
  
Internal Link::

  .. __simple-exampl-label:

  간단한 예제
  ===========

  어쩌고 저쩌고.... "간단한 예제"로 가는 링크를 :ref:`simple-example-label` 로 만들 수 있다.
  :ref:`label` 형태의 link 는 현재 파일 뿐 아니라 다른 파일에 존재하는 label 로도 링크할 수 있다.
  (즉 전체 문서상에서 label 이 고유해야 한다.)
  
  
:ref:`simple-example-label` 를 눌러보라


Toc tree::

  toc tree 는 Table Of Contents 즉 색인이란 뜻이다.
  .. toctree::
	 :maxdepth: 2

	 first_file
	 second_file

  first_file 과 second_file 에 있는 secton header 들을 2 단계까지 보여준다.
  

Other Tutorials
---------------
- `A ReStructuredText Primer <http://docutils.sourceforge.net/docs/user/rst/quickstart.html>`_
  

`emacs keybinding <http://docutils.sourceforge.net/docs/user/emacs.html#key-bindings>`_
---------------------------------------------------------------------------------------

- C-c C-a
  
  Commands to adjust the section headers and work with the hierarchy they build.
  C-c C-a C-a: 현재 line 을 section header 로 만든다
  
- C-c C-c
  
  Commands to compile the current reStructuredText document to various output formats.
  
- C-c C-l
  
  Commands to work with lists of various kinds.
  
- C-c C-r
  
  Commands to manipulate the current region.
  
- C-c C-t
  
  Commands to create and manipulate a table of contents.

- 위 명령어 + C-h: 관련 명령어들에 대한 설명을 볼 수 있다.



  

