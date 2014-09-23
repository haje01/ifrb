.. _plugin-opening:

구멍(Opening)
=============

구멍은 :ref:`plugin` 의 한 종류로, :ref:`thing` 가 :ref:`movement` 할 수 있는
통로이다. 단 방향으로만 이동한다.

.. seealso::
   :ref:`diagram-obj` 에서 Opening 를 보라.

.. note::
  구멍 플러그인을 가지는 물체를 간단히 '구멍' 으로 부르기도 한다.

**특징**

#. 구멍은 대상 :ref:`space` 한 방향으로만 이동한다.
#. 따라서 왕래를 하기위해서는 양쪽에 구멍이 필요하다.

*다음과 같은 속성을 가진다.*

.. _open:

열린(Open)
----------
열려있으면 참, 아니면 거짓

:ref:`type-boolean` 이고, 기본은 거짓

대상(Dest)
----------
이동할 대상 :ref:`space` 를 가르킨다.


*구멍에는 다음과 같은 종류가 있다.*

.. toctree::
   :maxdepth: 2

   opening/door
   opening/window

