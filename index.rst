.. ifrb documentation master file, created by
   sphinx-quickstart on Fri Sep 12 10:25:31 2014.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

IFRB에 온 것을 환영한다!
===================================

IFRB는 *Interactive Fiction Rule Book* 의 약자로 인터랙티브 픽션을 위한
규칙을 정의하는 문서이다. 여기에는 구현에 관한 내용은 포함하지 않는다.

서문
----

인터랙티브 픽션(Interactive Fiction, 이하 IF)는 가장 적은 리소스로 많은
컨텐츠를 담을 수 있는 소설과 유사한 미디어의 한 형태이다. 문자라는 최소한의
심볼을 가지고 구현되기에 그것은 다양한 형태(웹, 데스크탑/모바일 App 등)로 즐길
수 있다. 가급적 많은 디바이스를 지원하기 위해서 이 문서에서는 공통의 규칙만을
서술하고, 실제 구현은 각 구현체에 맡기는 방법을 선택하였다.


기본 객체들
-----------

.. toctree::
   :maxdepth: 2

   object
   spatial
   space
   thing
   character

고급 객체들
-----------

.. toctree::
   :maxdepth: 2

   script
   state
   type


플레이의 구성
-------------
:ref:`play` 는 크게 묘사를 읽고 행위를 하는 것으로 구성된다. 

.. toctree::
   :maxdepth: 2

   description
   action

기타
----

.. toctree::
   :maxdepth: 2

   sample
   diagram
   glossary

색인
====

* :ref:`genindex`

