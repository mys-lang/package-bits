|test|_

About
=====

Basic bits operations.

Project: https://github.com/mys-lang/package-bits

Examples
========

.. code-block:: python

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

Functions and types
===================

.. mysfile:: src/lib.mys

.. |test| image:: https://github.com/mys-lang/package-bits/actions/workflows/pythonpackage.yml/badge.svg
.. _test: https://github.com/mys-lang/package-bits/actions/workflows/pythonpackage.yml
