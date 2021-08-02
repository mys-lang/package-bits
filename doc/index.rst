|discord|_
|test|_
|stars|_

About
=====

Basic bits operations in the `Mys programming language`_.

Project: https://github.com/mys-lang/package-bits

Examples
========

.. code-block:: mys

   from bits import reverse
   from bits import leading_ones
   from bits import leading_zeros
   from bits import count_ones
   from bits import count_zeros
   from bits import rotate_left
   from bits import rotate_right

   def main():
       value: u32 = 0x12345678
       assert reverse(value) == 0x1e6a2c48
       assert leading_ones(value) == 0
       assert leading_zeros(value) == 3
       assert count_ones(value) == 13
       assert count_zeros(value) == 19
       assert rotate_left(value, 8) == 0x34567812
       assert rotate_right(value, 8) == 0x78123456

API
===

.. mysfile:: src/lib.mys

.. |discord| image:: https://img.shields.io/discord/777073391320170507?label=Discord&logo=discord&logoColor=white
.. _discord: https://discord.gg/GFDN7JvWKS

.. |test| image:: https://github.com/mys-lang/package-bits/actions/workflows/pythonpackage.yml/badge.svg
.. _test: https://github.com/mys-lang/package-bits/actions/workflows/pythonpackage.yml

.. |stars| image:: https://img.shields.io/github/stars/mys-lang/package-bits?style=social
.. _stars: https://github.com/mys-lang/package-bits

.. _Mys programming language: https://mys-lang.org
