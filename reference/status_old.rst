************************
Status API (Old Version)
************************

.. warning::
  The LineAPI is deprecated and has been replaced by the API
  of the status page itself. The EOL for the old Status API is
  the 1st June of 2017!


The Status API provides a overview of the current availability of miscellaneous Line-Lan services

api/status
----------

Gives back a full overview for the availability of all services.

Example request::

  https://api.line-lan.net/api/status/

Example result::

  Website: Online
  Database: Online
  Mail: Online
  API: Online
  Teamspeak: Online
  DNS: Online
  Ping: 15 ms

api/status/x
------------

Gives back the status of the specified service.

Example request::

  https://api.line-lan.net/api/status/api/

Example result::

  API: Online

