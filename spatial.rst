.. _spatial:

공간적 객체(Spatial)
====================
공간적 객체는 :ref:`object` 의 한 종류로, 공간을 차지하는 객체를 정의하기 위해 사용된다.

.. seealso::
   :ref:`diagram-obj`

*다음과 같은 속성이 있다.*

.. _location:

위치(Location)
--------------
:ref:`spatial` 는 :ref:`space` 에 소속될 수 있으며, 이 경우 그
:ref:`spaceparent` 를 **위치** 라 한다.

꼭 필요하지는 않으며, :ref:`spatial` 를 가리킨다.

.. note::
  위치는 계층적으로 구성되는 경우가 많다. 자신의 위치를 포함하는 위치들을
  **상위위치** 라고 부른다.

.. _boundary:

경계(Boundary)
--------------
:ref:`spatial` 가 차지하는 영역을 나타낸다. 정확한 공간 좌표가 필요하지는 않고
지도를 표시할 정도의 정확만 가진다.

꼭 필요하지는 않으며, :ref:`type-aabb` 이다.

.. _luminance:

조도(Luminance)
---------------

조도는 :ref:`spatial` 의 밝기를 나타내는데, 다음과 같은 규칙으로 결정된다.

#. 물체는 자신이 속한 :ref:`location` 의 조도를 고려한다.
#. 물체는 :ref:`part` 가 있는 경우 그것의 조도를 고려한다.
#. 물체는 :ref:`plugin-light` 이 있는 경우 그것의 조도를 고려한다.
#. :ref:`space` 은 :ref:`children` 의 조도를 고려한다.
#. 고려 대상 조도들 중 가장 밝은 것을 선택한다.

값은 :ref:`type-brightness` 이다.

비어 있음(Hollow)
-----------------

:ref:`type-boolean` 으로, 속이 비어 있는 :ref:`space` 나 :ref:`opening` 의 경우
참, 아니면 거짓이다.
