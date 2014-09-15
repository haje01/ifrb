.. _thing:

물체(Thing)
===========

물체는 :ref:`object` 의 한 종류로, :ref:`scenario` 에 등장하는 다양한 대상물을
말한다.

**특징**

#. 물체는 :ref:`luminance` 를 가진다.

*다음과 같은 속성이 있다.*

.. _transparent:

투명도(Transparent)
-------------------

:ref:`thing` 가 빛을 투과할 수 있는지 여부.

:ref:`type-boolean` 이며, 기본값은 거짓이다.

.. _part:

파트(Part)
----------
:ref:`thing` 를 구성하는 하나 이상의 하위 :ref:`thing` 를 파트로 가진다. 파트가
되는 객체는 이 객체를 :ref:`composite` 로 가진다.

하나 이상의 :ref:`thing` 을 가리킬 수 있다.

.. _plugin:

플러그인(Plugin)
----------------
플러그인은 :ref:`thing` 에 장착되어 객체의 기능을 확장하는 역할을 한다.

*다음과 같은 플러그인이 있다.*

.. toctree::
   :maxdepth: 2

   thing/plugin

하나 이상의 플러그인을 가질 수 있다.
