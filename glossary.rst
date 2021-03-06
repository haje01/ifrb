용어
====

.. _scenario:

시나리오(Scenario)
------------------
IF를 진행하기 위한 대본으로, 문학의 그것과는 달리 사실상 프로그램에 가깝다.

.. _author:

작가(Author)
------------
:ref:`scenario` 를 작성하는 사람.

.. _story:

스토리(Story)
-------------
IF의 :ref:`play` 결과로 만들어진 상태를 칭한다. 문학의 그것과는 달리 플레이하는
동안 계속 변한다.

.. _play:

플레이(Play)
------------
IF에서 유저가 :ref:`description` 을 읽고 명령을 내리는 것.

.. _map:

지도(Map)
---------
:ref:`play` 시 위치를 참고하고, 세계관에 몰읿할 수 있도록 하는 목적. 실제
지도처럼 정교하지는 않다. :ref:`spatial` 의 위치 와 크기, 연결 정보가 표시된다.

.. _direction:

방향(Direction)
---------------
방향은 동, 서, 남, 북과 아래/위의 6방이 있다.

.. _super:

슈퍼 객체(Super Object)
-----------------------
객체 지향에서 말하는 상속 개념에서 어떤 객체가 상속을 받은 모 객체.

.. _composite:

복합 물체(Composite)
--------------------
파트가 되는 객체에서 보았을 때 그것들이 이루어 내는 상위의 물체.

.. _ascendant:

조상(Ascendant)
---------------
:ref:`spatial` 가 자신을 포함하는 모든 상위 :ref:`parent` 를 가르키는 말.

후예(Descendant)
----------------
:ref:`space` 가 직/간접 자식을 포함하는 모든 :ref:`children` 을 가르키는 말.

.. _commonasc:

공통 조상(Common Ascendant)
------------------------------------
두 :ref:`spatial` 이 공유하는 :ref:`ascendant`.

.. _outerspace:

외부 공간(Outer Space)
----------------------
:ref:`spatial` 가 속한 :ref:`space` 을 말한다.

.. _innerspace:

내부 공간(Inner Space)
----------------------
:ref:`space` 혹은 물체 내부의(:ref:`plugin-container` 을 통한) :ref:`space` 의
안을 말한다.
