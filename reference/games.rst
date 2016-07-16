*********
Games API
*********

This part of the LineAPI provides access to the Game list of the event managment software.

api/games
---------

Gives back a full list of all registered games.

Example request::

  https://api.line-lan.net/api/games/

Example result::

  Half-Life 
  Counter-Strike 1.6 
  Unreal Tournament 
  Warcraft III 
  Warcraft III: Frozen Throne 
  Battlefield 1942 
  Counter-Strike: Source 
  League of Legends 
  Dota 
  Dota 2 
  Half-Life Deathmatch 
  Half-Life 2 
  Half-Life 2 Deathmatch 
 
  etc...

.. warning::
  Currently, over 150 games are in this database, expanding with new releases. So this list can get quite large.

api/games/x
-----------

Gives back the name for the specified gameid.

Example request::

  https://api.line-lan.net/api/games/7/

Example result::

  Counter-Strike: Source 

