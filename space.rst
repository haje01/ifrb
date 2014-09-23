.. _space:

공간(Space)
============

공간은 :ref:`spatial` 의 한 종류로, 비어 있어서 다른 :ref:`spatial` 가 들어갈
수 있다.

.. seealso::
   :ref:`diagram-obj` 의 Space 를 보라.

**특징**

#. 공간은 다른 공간이나 방을 :ref:`children` 로 가질 수 있다.
#. 한 공간에서 다른 공간, 또는 :ref:`room` 으로 :ref:`movement` 할 수 있다.
#. 공간에서 다른 공간으로의 이동은 :ref:`name` 을 지정해서 한다.

*다음과 같은 속성이 있다.*

.. _children:

자식들(Children)
------------------
공간에 속하는 하나 이상의 :ref:`spatial` 들을 그 공간의 자식들이라고 한다.
공간의 자식들은 이 공간을 :ref:`outerspace` 로 가진다.

.. seealso::
   :ref:`diagram-obj` 에서 Space 에서 Spatial 로의 children 집합 관계를 보라.

.. _room:

방(Room)
========

방은 :ref:`space` 의 한 종류로, IF의 가장 흔한 공간이다.

.. seealso::
   :ref:`diagram-obj` 에서 Room 을 보라.

**특징**

#. 방은 :ref:`space` 을 자식으로 가질 수 없다.
#. 방은 :ref:`direction` 별로 :ref:`door` 을 가질 수 있고, 이것을 통해서 다른
   방 또는 :ref:`space` 으로 :ref:`movement` 한다.

.. note:
   공간으로 나가는 방문을 출구, 공간에서 들어오는 방문을 입구라고 한다.

