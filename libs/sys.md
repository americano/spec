# Sys library
_Core functions_

## Argument Parsing
Argument parsing, for defining options during command-line execution of a program.

Parse argument **via:**

	import sys
	print sys.arg['name']

So it would return if a `-name` flag was passed or not, and any text after it before the next flag

###Or:

	import sys
	print args[2]

Which prints the 3rd argument, an argument delimiter via a space

###Or:

	import sys
	print sys.argRaw

Which is a string of all of the arguments passed, as they were passed
