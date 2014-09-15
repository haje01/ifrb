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

first time run
    이 조건이 실행된 것이 최초인가?

호출자 관련
-----------

call by cpu
    이 :ref:`script` 의 실행이 CPU에 의한 것인가? 첫 번째 호출 뎁스로 판단한다.


공간적 객체 관련
----------------

[spatial] pitch dark
    :ref:`spatial` 가 깜깜한 곳에 있는가?


지역 관련
---------

[regional] space dark
    :ref:`regional` 의 :ref:`space` 이 깜깜한가?

[regional] contains 
    :ref:`regional` 가 :ref:`spatial` 을 가지고 있는가?


물체 관련
----------
[thing] switch on
    :ref:`plugin-switch` 이 켜졌는가?

[thing] light on
    :ref:`plugin-light` 이 켜졌는가?

[thing] covered by [spatial]
    물체가 특정 :ref:`spatial` 로 감싸지는가?

[thing] location is [spatial]
    물체가 특정 :ref:`spatial` 에 정확히 :ref:`location` 하는가?

[thing] composed by [thing]
    물체가 특정 :ref:`thing` 을 :ref:`part` 로 가지는가?

[thing] contains [thing]
    :ref:`thing` 에 :ref:`plugin-container` 이 있고, :ref:`thing` 를 가지는가?


캐릭터 관련
-------------
[character] visible [thing]
    플레이어가 특정 :ref:`thing` 을 볼 수 있는가?

[character] gettable [thing]
    플레이어가 특정 :ref:`thing` 을 얻을 수 있는가?
