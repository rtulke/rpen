rpen
====

rpen (Red Pencil) is a comandline text highlighter based on egrep

Requirements:
-------------

* Python 2.5 or higher
* egrep or grep 

Installation:
-------------
* download rpen.py or use git:

<code>
$ git clone https://github.com/rtulke/rpen.git
$ cp rpen/rpen.py /usr/local/bin/rpen
$ chmod 777 /usr/local/bin/rpen (systemwide)
</code>

Examples:
---------
<code>
$ cat /foo/bar | rpen searchstring1 searchstring2 .. 
</code>


or try less with RAW mode

<code>
$ cat /foo/bar | rpen searchstring1 searchstring2 .. | less -R 
</code>


rpen with regex:

<code>
$ cat /foo/bar | rpen ^.*[04]
</code>


highlight whole line:

<code>
$ cat /foo/bar | rpen ^.\*searchstring\*.$
</code>


if first arg i --> case_insensitive:

<code>
$ cat /foo/bar | rpen i Searchstring1 searchString2 .. | less -R 
</code>

