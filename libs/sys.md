# Sys library
_Core functions_

## Argument Parsing
Argument parsing, for defining options during command-line execution of a program.

Parse argument **via:**

	import sys
	print sys.arg['name']

Returns if "--name" flag was passed or not (true/false), and any text attached(str).

###Or:

	import sys
	print sys.args[2]

Which prints the 3rd argument passed(str).

###Or:

	import sys
	print sys.argRaw

Which is a string of all of the arguments passed(str).
