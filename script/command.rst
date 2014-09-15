.. _command:

명령(Command)
=============
유저는 디바이스 상의 UI를 선택하여 :ref:`story` 에 영향을 미치는 :ref:`action`
를 만들어 낼 수 있다.


물체 관련
---------

move [thing] to [area | room | thing]
    특정 :ref:`thing` 를 대상 물체의 :ref:`area`, :ref:`room` 혹은 :ref:`thing`
    로 이동한다. 대상 물체에 :ref:`plugin-container` 이 없으면 예외 발생.

make [thing] part of [thing]
    특정 :ref:`thing` 를 대상 물체의 :ref:`part` 가 되게 한다.

hide(show) [thing]
    특정 :ref:`thing` 를 보이지 않게(보이게) 한다.

[thing] light on(off)
    물체의 라이트를 끈다(켠다). 대상 물체에 :ref:`plugin-light` 가 없으면 예외
    발생.

[thing] switch on(off)
    물체의 스위치를 끈다(켠다). 대상 물체에 :ref:`plugin-switch` 가 없으면 예외
    발생.
