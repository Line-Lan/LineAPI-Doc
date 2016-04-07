*********
Users API
*********

This part of the LineAPI provides access to the user database of the Line-Lan event managment.
You can acces Userdata like names, benchmarks, rigs etc.

api/users
---------

Gives back a list of all registered usernames.

Example usage::

  file_get_contents('https://api.line-lan.net/api/users/')

Example Result::

  user1
  user2
  user3
  user4
  user5
  
  etc.

.. note::
	You can use /api/users/x/ if you want the username to a known userid you know instead of using line-numbers.

api/users/x
-----------

Like /api/users/, but only gives back the name of the user with the userid specified as x.

Example usage::

  file_get_contents('https://api.line-lan.net/api/users/15/')

Example Result::

  user15

with user15 corresponding to the name of the 15th registered user in the database.

api/users/x/name
----------------

Gives back the first and last name of a user.

Example usage::

  file_get_contents('https://api.line-lan.net/api/users/5/name/')

Example Result::

  firstname
  lastname

api/users/x/rig
---------------

Gives back the details of the Computer *(aka. rig)* of the user with the userid x.

.. note::
  A RAW-version of this command is available. See :doc:`Syntax Page </syntax>` for details.

Example usage::

  file_get_contents('https://api.line-lan.net/api/users/1/rig/')

Example Result::

  Intel Core-i5 3330 @3000 Mhz
  4 GB DDR3
  Intel HD Graphics 2500
  2000 GB

api/users/x/clan
----------------

Gives back the clan of a user.

Example usage::

  file_get_contents('https://api.line-lan.net/api/users/5/clan/')

Example Result::

  The Defenders

api/users/x/quote
-----------------

Gives back the quote of a user.

Example usage::

  file_get_contents('https://api.line-lan.net/api/users/3/quote/')

Example Result::

  coffee is my water!

api/users/x/benchmarks
----------------------
Gives back the benchmark results of a user.

.. note::
  A RAW-version of this command is available. See :doc:`Syntax Page </syntax>` for details.

Example usage::

  file_get_contents('https://api.line-lan.net/api/users/5/name/')

Example Result::

  3DMark Cloud Gate 1234
  3DMark Fire Strike 4567
  3DMark Ice Storm 6789
  3DMark Sky Diver 4321
  PCMark 8 Home 9876

