***************
Troubleshooting
***************

There are a lot of factors that can lead to a failiure of the request. The most common ones are listed below

Misspelled Requests
-------------------

Often you just make a mistake in spelling the Request URI correctly. Watch out for typing errors! This is the most common error.

.. tip::
 You can copy the URI in a web browser. If you get a response everything works fine on server side.

Incombatible get method
-----------------------

As described in the :doc:`Requirements <requirements>`, you have to use a programming/scripting language that allows you to use GET requests on HTTP and HTTPS streams.

Scripts with JSON-only input
----------------------------

As you might have noticed, this API does **not** deliver its data in the JSON formats. There are many premade scripts/Frameworks that rely on a JSON-output, but imo a minimal response with just the requested data is easier to use, so we went with that

HTTP 5xx-Responses
------------------

If you get 500, 510, 522 etc. responses back from the server, check that the API-Server is available.

.. note::
 Visit https://status.line-lan.net for detailed information about uptime
