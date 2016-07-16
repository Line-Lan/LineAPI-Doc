***************
Tournaments API
***************

This part of the LineAPI provides access to the tournaments of the Line-Lan eventpage


api/tournaments
---------------

Gives back a list of all existing tournaments.

Example request::

  https://api.line-lan.net/api/tournaments/

Example result::

  Turnier1
  Turnier2
  ...
  
api/tournaments/x
-----------------

Gives back the name of the specified tournament

Example request::

  https://api.line-lan.net/api/tournaments/2/

Example result::

  Turnier2

api/tournaments/x/type
----------------------

Gives back the type of the specified tournament

Example request::

  https://api.line-lan.net/api/tournaments/1/type/

Example result::

  single elimination

api/tournaments/x/game
----------------------

Gives back the game of the specified tournament

Example request::

  https://api.line-lan.net/api/tournaments/1/game/

Example result::

  Counter-Strike: Source
  
api/tournaments/x/teamcount
---------------------------

Gives back the maximum number of teams of the specified tournament

Example request::

  https://api.line-lan.net/api/tournaments/1/teamcount/

Example result::

  16
  
api/tournaments/x/teamsize
--------------------------

Gives back the teamsize of the specified tournament

Example request::

  https://api.line-lan.net/api/tournaments/1/teamsize/

Example result::

  5

api/tournaments/x/notes
-----------------------

Gives back the notes and rules of the specified tournament

Example request::

  https://api.line-lan.net/api/tournaments/1/notes/

Example result::

  MR 30
  Round time 1:45
  bomb time 0:45
  no scripts allowed!
  ...

api/tournaments/x/settings
--------------------------

Gives back the server settings of the specified tournament

Example request::

  https://api.line-lan.net/api/tournaments/1/notes/

Example result::

  sv_cheats 0
  sv_pure 1
  time_round 105
  time_defuse 45
  ...




