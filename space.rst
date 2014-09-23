.. _space:

공간(Space)
============

공간은 :ref:`spatial` 의 한 종류로, 비어 있어서 물체가 들어갈 수 있다.

.. seealso::
   :ref:`diagram-obj` 의 Space 를 보라.

**특징**

#. :ref:`spatial` 는 공간을 통해서 자식 :ref:`thing` 를 가진다.
#. 공간은 단독으로 있지 못하고, :ref:`regional` 혹은 물체의
   :ref:`plugin-container` 안에 존재할 수 있다. 이것을 :ref:`spaceparent`
   라고 한다.
#. 공간 그 자체는 이동할 수 없다.
#. 공간은 :ref:`luminance` 를 가진다.

*다음과 같은 속성이 있다.*

.. _spacechild:

공간의 자식 객체(Spatial Child of Space)
-------------------
공간에 속하는 하나 이상의 :ref:`spatial` 를 그 **공간의 자식 객체** 라고 한다.
공간의 자식 객체는 이 공간을 :ref:`outerspace` 로, 이 :ref:`spaceparent` 를
:ref:`location` 으로 가진다.

.. seealso::
   :ref:`diagram-obj` 에서 Spatial 간의 Location 집합 관계, 그리고 Spatial 에서
   Space 로의 OuterSpace 집합 관계를 보라.
