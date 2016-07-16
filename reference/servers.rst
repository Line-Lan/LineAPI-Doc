***********
Servers API
***********

This part of the LineAPI provides access to the serverlist of the managment software.

.. warning::
  The servers connected to tournaments are found in the Tournaments API.

api/server
----------

Gives back a list of all registered servers.

Example request::

  https://api.line-lan.net/api/server/

Example result::

  64.74.97.72:27017 Counter-Strike: Source
  91.211.116.28:27015 Counter-Strike 1.6

.. note::
  A RAW-version of this command is available. See :doc:`Syntax Page </syntax>` for details.

api/server/x
------------

Gives back the details of a specified server.

Example request::

  https://api.line-lan.net/api/server/2/

Example result::

  91.211.116.28:27015,Counter-Strike 1.6

.. note::
  This Request should deliver RAW-Compatible data. See :doc:`Syntax Page </syntax>` for details.

