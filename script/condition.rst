.. _condition:

조건(Condition)
===============

특정한 조건이 맞는지 여부를 검사한다. 다음과 같은 다양한 조건들이 있다.

.. _cond_always:

단순 조건
----------

always
    항상 참이다.

never
    항상 거짓이다.

시간 관련
----------

first time
    이 조건이 실행된 것이 최초인가?

호출자 관련
-----------

call by cpu
    이 :ref:`script` 의 실행이 CPU에 의한 것인가? 첫번째 호출 뎁스로 판단한다.


물체 관련
-----------
switch on
    :ref:`switch` 이 켜졌는가?

light on
    :ref:`light` 이 켜졌는가?

thing space dark
    :ref:`thing` 의 공간이 깜깜한가?

thing covered by
    특정 공간으로 감싸지면 참 

thing at
    특정 공간에 정확히 위치할 때만 참


플레이어 관련
-------------
player space dark
    :ref:`player` 의 공간이 깜깜한가?

player covered by
    플레이어가 특정 공간에 포함되는가?
    특정 공간으로 감싸지면 참 

player at
    특정 공간에 정확히 위치할 때만 참