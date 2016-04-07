********
News API
********

This part of the LineAPI provides access to the news feature of the Line-Lan event managment.

.. warning::
  This is **NOT** the API for the Line-Lan.net homepage/blog. Use the RSS-Feed or the WordPress-API instead if you want to interact with those.

api/news
--------

Gives back a list of all published news articles.

Example usage::

  file_get_contents('https://api.line-lan.net/api/news/')

Example Result::

 Line-Lan Eventmanagment

 This is the software we're going to be using to coordinate the flow of information. We have a variety of things  going on here, but here are a few hints for the website: 1. If you see this icon: HLSW next to a server ip, you can click on it to launch HLSW to connect to the server. HLSW is a multi-game server connection tool. To join a game using HLSW, click the icon, and it will bring up the IP address in the HLSW window. Hit enter, right click on the server in the server list and click on Connect. It will make it much easier to join tournament servers. 2. You're free to participate in the other events we have available: The Marathon Global Tournament TournamentsBenchmarking Competition

api/news/x
----------

Gives back a the news article with the specified newsid *(x)*.

Example usage::

  file_get_contents('https://api.line-lan.net/api/news/3/')

Example Result::

  Test message
  
  This is the third message of this news database!
