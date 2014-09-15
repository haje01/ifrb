.. _type:

타입
====

여기에서는 :ref:`scenario` 작성시 사용되는 타입들을 소개한다.

.. _type-boolean:

불린(Boolean) 타입
------------------

참 또는 거짓

.. _type-string:

문자열 타입
-----------
UTF-8 인코딩의 유니코드 문자열.

.. _type-id:

ID 타입
-------
레귤러 익스프레션 ``[_a-zA-Z][_a-zA-Z0-9]{0,30}`` 을 따르는 문자열

.. _type-aabb:

축정렬 경계박스(AABB ) 타입
---------------------------
공간상의 최대 좌표와 최소 좌표를 가지는 타입

.. _type-brightness:

밝기(Brightness) 타입
---------------------
미정의(Undefined), 밝음(Bright), 어두움(Dim), 깜깜함(Pitch-dark)의 나열값을
가진다.
