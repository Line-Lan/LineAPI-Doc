**********
Status API
**********

.. note::
  Note: This is the new json version of the status API

The Status API provides a overview of the current availability of miscellaneous Line-Lan services

api
---

Returns the availability of all services and some status info

Example request::

  https://status.line-lan.net/api/

Example result::

  {
    "http_code": 200,
    "date": "Mon, 17 Apr 2017 12:11:27 +0200",
    "availability": "full",
    "all_avialable": true,
    "latency": 48,
    "server_total": 6,
    "server_up": 6,
    "server_down": 0,
    "server_up_percentage": 100,
    "servers": [
        {
            "display": "Homepage",
            "address": "line-lan.net",
            "port": 443,
            "available": true
        },
        {
            "display": "Database",
            "address": "localhost",
            "port": 3306,
            "available": true
        },
        {
            "display": "Mail",
            "address": "mail.line-lan.net",
            "port": 993,
            "available": true
        },
        {
            "display": "Minecraft",
            "address": "mc.line-lan.net",
            "port": 25565,
            "available": true
        },
        {
            "display": "Teamspeak",
            "address": "ts.line-lan.net",
            "port": 10011,
            "available": true
        },
        {
            "display": "DNS",
            "address": "kevin.ns.cloudflare.com",
            "port": 53,
            "available": true
        }
    ]
}

api/ping
--------

Returns the currentping  latency of the main server

Example request::

  https://status.line-lan.net/api/ping/

Example result::

 {
    "http_code": 200,
    "date": "Mon, 17 Apr 2017 12:14:05 +0200",
    "latency": 17
}

api/status
----------

Returns the status of all services without additional information

Example request::

  https://status.line-lan.net/api/status/

Example result::

  {
    "http_code": 200,
    "date": "Mon, 17 Apr 2017 12:12:26 +0200",
    "servers": [
        {
            "display": "Homepage",
            "address": "line-lan.net",
            "port": 443,
            "available": true
        },
        {
            "display": "Database",
            "address": "localhost",
            "port": 3306,
            "available": true
        },
        {
            "display": "Mail",
            "address": "mail.line-lan.net",
            "port": 993,
            "available": true
        },
        {
            "display": "Minecraft",
            "address": "mc.line-lan.net",
            "port": 25565,
            "available": true
        },
        {
            "display": "Teamspeak",
            "address": "ts.line-lan.net",
            "port": 10011,
            "available": true
        },
        {
            "display": "DNS",
            "address": "kevin.ns.cloudflare.com",
            "port": 53,
            "available": true
        }
    ]
}

api/status/x
------------

Returns the status of a specified server

Example request::

  https://status.line-lan.net/api/status/homepage/

Example result::

  {
      "http_code": 200,
      "date": "Mon, 17 Apr 2017 12:15:54 +0200",
      "display": "Homepage",
      "address": "line-lan.net",
      "port": 443,
      "available": true
  }