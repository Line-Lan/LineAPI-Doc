**********
Status API
**********

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

