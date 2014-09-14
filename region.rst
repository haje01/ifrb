.. _region:

지역(Region)
============

지역은 :ref:`node` 의 한 종류로, :ref:`scenario` 의 배경이 되는 큰 장소를 말한다.

**특징**

#. 지역에는 :ref:`space` 이 있다.
#. 지역 그 자체는 이동할 수 없다.

지역은 넓이에 따라 구역, 건물, 방으로 나뉜다.

.. _area:

구역(Area)
----------
구역은 :ref:`region` 의 한 종류로, 가장 큰 지역이다.

**특징**

#. 한 구역에서 다른 구역, 또는 :ref:`room` 으로 :ref:`movement` 할 수 있다.


.. _structure:

건물(Structure)
---------------

건물은 :ref:`region` 의 한 종류로, 주로 다수의 방을 그룹짓고, 그것을 구역에서
:ref:`description` 하기 위해 사용된다.

**특징**

#. 건물은 :ref:`area` 공간의 자식으로만 존재할 수 있다.
#. 건물의 :ref:`space` 은 다른 건물이나 :ref:`room` 을 자식 공간으로 가질 수 있다.


.. _room:

방(Room)
--------

방은 :ref:`region` 의 한 종류로, IF의 가장 흔한 공간이다.

**특징**

#. 방은 속한 지역없이 독자적으로 존재할 수 있다. 
#. 방의 :ref:`space` 은 다른 :ref:`region` 을 자식으로 가질 수 없다.
#. 방의 :ref:`space` 는 :ref:`direction` 별로 :ref:`door` 을 가질 수 있고, 이것을 통해서 다른
   방 또는 :ref:`region` 으로 :ref:`movement` 한다.

.. note:
   구역으로 나가는 방문을 출구, 구역에서 들어오는 방문을 입구라고 한다.

