.. _thing:

물체(Thing)
===========

물체는 :ref:`spatial` 의 한 종류로, :ref:`scenario` 에 등장하는 다양한 대상물을
말한다.

.. seealso::
   :ref:`diagram-obj` 에서 Thing 을 보라.

**특징**

#. 물체는 :ref:`luminance` 를 가진다.
#. :ref:`thing` 는 현재 공간에서 다른 공간으로 :ref:`movement` 이 가능하다.

*다음과 같은 속성이 있다.*

.. _transparent:

투명도(Transparent)
-------------------

:ref:`thing` 가 빛을 투과할 수 있는지 여부.

:ref:`type-boolean` 이며, 기본값은 거짓이다.

.. _part:

파트(Part)
----------
:ref:`thing` 를 구성하는 하나 이상의 하위 :ref:`thing` 를 **파트** 로 가질 수
있다. 파트가 되는 객체는 상위 객체를 :ref:`composite` 로 가진다.

.. seealso::
   :ref:`diagram-obj` 에서 Thing 간의 Part 집합 관계를 보라.

물체는 하나 이상의 :ref:`thing` 을 파트로 가리킬 수 있다.

.. _plugin:

플러그인(Plugin)
----------------
플러그인은 :ref:`thing` 에 장착되어 물체의 기능을 확장하는 역할을 한다.

.. seealso::
   :ref:`diagram-obj` 에서 Plugin 에서 Thing 으로의 합성 관계를 보라.


*다음과 같은 플러그인이 있다.*

.. toctree::
   :maxdepth: 2

   plugin/switch
   plugin/light
   plugin/container
   plugin/opening

물체는 하나 이상의 플러그인을 가질 수 있다.
