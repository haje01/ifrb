.. _opening:

구멍(Opening)
=============

구멍은 :ref:`spatial` 의 한 종류로, 비어 있어서 두 :ref:`spatial` 을 이어준다.

**특징**

#. 구멍은 A/B 두 객체가 하나의 객체를 이룬다.
#. A/B는 각각 연결된 두 :ref:`spatial` 을 :ref:`location` 으로 가진다.
#. A로 들어가면 B로 :ref:`movement` 하고, B로 들어가면 A로 이동한다.

.. note::
   내/외라는 표현도 가능하겠으나, 혼란을 줄이기 위해 A/B로 부르겠다.

.. _door:

문(Door)
----------
문은 :ref:`opening` 의 한 종류로, :ref:`character` 가 서서 :ref:`spatial` 을 이동할 수
있는 통로이다.

.. _window:

창문(Window)
------------
창문은 :ref:`opening` 의 한 종류로, :ref:`door` 과 유사하나 크기가 작고 대개 빛이
통과하는 :ref:`transparent` 을 가진다.
