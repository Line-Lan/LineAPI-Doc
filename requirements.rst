************
Requirements
************

Basics
------

The only real requirement for the usage of the LineAPI is that your Client must have a active internet connection and must be able to recieve data via a secure connection (HTTPS).

HTTPS
-----

As it is likely that you work with sensitive data over the LineAPI, we decided to only allow connections via HTTPS. We took this step because the development of the web is 
rapidly changing what can lead to security problems.
To adress these, a requirement for a secure connection should be the right decision.

.. note::
	For legacy reasons we allow older encryption standards to connect. But remember:
	Always use the strongest encryption available.


Optional: A explode()-like method
---------------------------------

Although it is not a requirement, your programming language should have a function that is able to create a array from a string by dividing it at a specified character, in our case a comma. This is useful when working with RAW-Data.

.. note::
	You can find more information about our Syntax in the :doc:`Syntax <syntax>` section

Recommendations
---------------

If you are new to programming and scripting in general, we recommend that you try php as it's easy to learn and relatively simple. php is pre-installed on most web-servers, so building your own web application based on the LineAPI should be no problem.

.. tip::
  You can find the php-manual at http://php.net/manual
