# Sys library
_Core functions_

## Argument Parsing
Argument parsing, for defining options during command-line execution of a program.

Parse argument *bob* **via:**

	import sys
	print sys.args['name']

Or **prettier:**

	import sys.args as arg
	print args['name']
    