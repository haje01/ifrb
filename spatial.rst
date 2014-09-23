.. _spatial:

공간적 객체(Spatial)
====================
공간적 객체는 :ref:`object` 의 한 종류로, 공간을 차지하는 객체를 정의하기 위해 사용된다.

.. seealso::
   :ref:`diagram-obj` 에서 Spatial 을 보라.

*다음과 같은 속성이 있다.*

.. _parent:

부모(Parent)
--------------
:ref:`spatial` 가 다른 공간적 객체에 속하면 그것을 **부모** 라고 한다.

.. seealso::
   :ref:`diagram-obj` 에서 Spatial 간의 Parent 집합 관계를 보라.

꼭 필요하지는 않으며, :ref:`spatial` 를 가리킨다.

.. _boundary:

경계(Boundary)
--------------
:ref:`spatial` 가 차지하는 영역을 나타낸다. 정확한 공간 좌표가 필요하지는 않고
:ref:`map` 를 표시할 정도의 정확만 가진다.

꼭 필요하지는 않으며, :ref:`type-aabb` 이다.

.. _luminance:

조도(Luminance)
---------------

조도는 :ref:`spatial` 의 밝기를 나타내는데, 다음과 같은 규칙으로 결정된다.

#. :ref:`spatial` 는 자신의 :ref:`parent` 의 조도를 고려한다.
#. :ref:`thing` 는 :ref:`parts` 가 있는 경우 그것의 조도를 고려한다.
#. 물체는 :ref:`plugin-light` 이 있는 경우 그것의 조도를 고려한다.
#. 물체는 :ref:`plugin-container` 이 있는 경고 :ref:`transparent` 가 참인 경우
   :ref:`children` 의 조도를 고려한다.
#. :ref:`space` 은 :ref:`children` 의 조도를 고려한다.
#. 고려 대상 조도들 중 가장 밝은 것을 선택한다.

값은 :ref:`type-brightness` 이다.
