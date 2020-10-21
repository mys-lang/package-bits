|buildstatus|_

Bits
====

Basic bits operations in the `Mys programming language`_.

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
       assert_eq(reverse(value), 0x1e6a2c48)
       assert_eq(leading_ones(value), 0)
       assert_eq(leading_zeros(value), 3)
       assert_eq(count_ones(value), 13)
       assert_eq(count_zeros(value), 19)
       assert_eq(rotate_left(value, 8), 0x34567812)
       assert_eq(rotate_right(value, 8), 0x78123456)

.. code-block:: text

   $ mys run

.. |buildstatus| image:: https://travis-ci.com/eerimoq/mys-bits.svg?branch=master
.. _buildstatus: https://travis-ci.com/eerimoq/mys-bits

.. _Mys programming language: https://github.com/eerimoq/mys
