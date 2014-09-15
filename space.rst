.. _space:

공간(Space)
============

공간은 :ref:`spatial` 의 한 종류로, 비어 있어서 물체가 들어갈 수 있다.

**특징**

#. 공간에는 :ref:`children` 가 있다.
#. :ref:`thing` 는 현재 공간에서 다른 공간으로 이동이 가능하다.
#. 공간 그 자체는 이동할 수 없다.
#. 공간은 :ref:`luminance` 를 가진다.

*다음과 같은 속성이 있다.*

.. _children:

자식 객체(Children)
-------------------
이 공간에 속하는 하나 이상의 :ref:`spatial` 자식객체 로 가진다. 자식객체는 이 공간을 :ref:`location` 으로 가진다.

.. _cover:
