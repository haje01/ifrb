.. _state:

상태(State)
===========

상태는 :ref:`object` 들 간의 관계, 혹은 :ref:`story` 의 상황을 나타낸다. 각 상태는
그것을 정의하는 조건들이 있고, 이 조건들을 모두 만족하면 성립한다.

*다음과 같은 상태들이 있다.*


.. _transmittable:

빛이 전송 가능한(Transmittable)
-------------------------------
:ref:`state` 의 한 종류로, 두 :ref:`spatial` 사이에서 빛이 전송 가능한지
나타낸다. 다음과 같이 결정된다.

#. 둘 다 물체이고 같은 :ref:`location` 에 있으면 가능.
#. 어느 한쪽이 물체인데 :ref:`transparent` 가 없고 :ref:`opencontainer`
   상태도 아닌 컨테이너 안에 있으면 불가.
#. 둘 다 물체이고 각 :ref:`location` 가 서로 다른 :ref:`room` 일때,
   두 방이 :ref:`door` 으로 연결되어 있지 않거나 문이 :ref:`opendoor` 상태가 아니면
   불가.
#. 둘 다 물체이고 한 :ref:`location` 는 :ref:`area` 다른 위치는
   :ref:`room` 일때, 그 방이 그 구역에 연결되어 있지 않거나 :ref:`opendoor` 상태가
   아니면 불가.
#. 이외는 가능.

결정된 값은 :ref:`type-boolean` 이다.

.. _visible:

볼 수 있는(Visible)
-------------------

:ref:`state` 의 한 종류로, :ref:`character` 가 대상 :ref:`thing` 을 볼 수
있는지 나타낸다.  다음과 같이 결정된다.

#. 캐릭터와 대상 물체가 :ref:`transmittable` 상태가 아니면 불가.
#. 캐릭터 혹은 대상 물체의 :ref:`luminance` 가 깜깜하면(Pitch-dark) 불가.
#. 이외는 가능.

결정된 값은 :ref:`type-boolean` 이다.

.. note::
   가시도의 대상은 물체뿐만 아니라 공간에 대해서도 결정된다.

.. _gettable:

얻을 수 있는(Gettable)
----------------------

:ref:`state` 의 한 종류로, :ref:`character` 가 대상 :ref:`thing` 를 얻을 수
있는지 나타낸다.  다음과 같이 결정된다.

#. 캐릭터와 대상 객체가 :ref:`visible` 상태가 아니면 불가.
#. 같은 :ref:`lowcommonloc` 가 없거나 :ref:`room` 보다 큰 것이면 불가.
#. 물체가 :ref:`opencontainer` 상태가 아닌 컨테이너 안에 있으면 불가.
#. 이외는 가능.
