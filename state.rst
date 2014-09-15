.. _state:

상태(State)
===========

상태는 :ref:`object` 들 간의 관계, 혹은 :ref:`story` 의 상황을 나타낸다. 각 상태는
그것을 정의하는 조건들이 있고, 이 조건들을 모두 만족하면 성립한다.

*다음과 같은 상태들이 있다.*

.. _visible:

볼 수 있는(Visible)
-------------------

볼 수 있는 것은 :ref:`state` 의 한 종류인데, :ref:`character` 가 대상 :ref:`spatial`
 를 볼 수 있는 지 나타낸다.  다음과 같이 결정된다.

#. 캐릭터가 위치한 :ref:`space` 의 :ref:`luminance` 가 깜깜하면 불가.
#. 대상 물체의 :ref:`luminance` 가 깜깜하면 불가.
#. 캐릭터와 대상 객체 사이에 :ref:`transparent` 가 없는 물체가 있으면 불가.
#. 이외의 경우 성립.

결정된 값은 :ref:`type-boolean` 이다.

.. note::
   가시도의 대상은 물체뿐만 아니라 공간에 대해서도 결정된다.


.. _reachable:

닿을 수 있는(Reachable)
-----------------------

닿을 수 있는 것은 :ref:`state` 의 한 종류인데, :ref:`character` 가 대상
:ref:`spatial` 에 접촉할 수 있는 지를 나타낸다. 다음과 같이 결정된다.

#. 캐릭터와 대상 객체의 :ref:`location` 가 다르면 불가.
#. 캐릭터와 대상 객체가 :ref:`visible` 상태가 아니면 불가.
#. 이외의 경우 성립.

