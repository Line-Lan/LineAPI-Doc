******
Syntax
******

We mainly use two different types of syntax for the responses:

* A human-readable format
* A computer-readable format

The human-readable format is intended to be used directly as a output, i.e::

   $result = file_get_contents('https://api.line-lan.net/api/users/1/rig/');
   echo($result);

.. note::
  All examples of codes in this manual are written in **PHP**. Therefor the usage in *(your preferred language)* may vary.

Human-readable format
---------------------

The Output of this would look like::

   Intel Core-i5 3330 @3000 Mhz
   4 GB DDR3
   Intel HD Graphics 2500
   2000 GB

As you can see, this type of formatting is quite easy to understand and could be outputted directly to the user.

Computer-readable format
------------------------

Often you don't want to output the data directly to thr user and rather process it before outputting. Therefor we deliver the data in our so-called RAW-Format.

.. tip::
   To access the RAW-Version of a request you can simpy add **/raw/** to the end of the url.

.. warning::
   Because not every Command has and/or needs this format the commands that have it are marked in the API reference.

The RAW-Version is simply a dump of the requested data, seperated by commas. To use it effetively, you have to split it first::

   $result = file_get_contents('https://api.line-lan.net/api/users/1/rig/');
   echo("$result");

This would result in something like::

  Intel,Core-i5 3330,3000,4,DDR3,Intel,HD Graphics 2500,2000

To use this output effectively, you could type::

	$splitted = explode(",",$result,10);

This creates the Array $Splitted which contains all data, identified whíth indicies beginning with 0::

   0 => Intel
   1 => Core-i5 3330,
   2 => 3000
   3 => 4
   4 => DDR3
   5 => Intel
   6 => HD Graphics 2500
   7 => 2000

Now you can access the requested data via the array.

Alternatives to PHP's explode() for other languages
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Java::

  String[] split = result.split(",");

C/C++::

  char *tok;
  char *src = malloc(strlen(srcStr) + 1);
  memcpy(src, srcStr);

  tok = strtok(src, ",");
  if(tok == NULL) {
  	printf("no tokens found");
  	free(src);
  	return ???;
  }
  printf("%s ; ", tok);
  while((tok = strtok(NULL, ",")))
  printf("%s ; ", tok);
  printf("\n");
  free(str);

Python::

  import result
  string.split(result, ',')

Others:

	Google: explode() in *language*
