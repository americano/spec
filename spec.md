#Core spec

The specification within this document has a relevant `README.md` for information about this file and surrounding repository. Things needing to be done are in `_Todo.md`, and this file uses the License within `LICENSE.md`.

## Hello World

### Braced
	init Main {
		print("Hello World!");
	}
### Cleansed
	init Main
		print "Hello World!"

## Variable declaration
### Integer
Non-decimal number

	int integervarthingy = 3
	
### Float
Decimal number

	float floatvarthingy = 3.5
	
### String
An alphanumerical string, wrapped in phrase marks.

	str stringvarthingy = "Stringy Thingy" 
	
### Array
A basic array.

	int[] arrayvarthingy = [1,2,3,4,5]
	
The array is singularly typed: an array of just int's, just str's, etc.

## Functions and Core procedures

### Declare a function
A basic function.

**Declare w/ braces:**

    func myFunction (arg,etc) {
        return lol;
    }

**Declare w/ cleanliness:**

    func myFunction arg,etc
        return lol

### Execute a function
Using a function.

**Declare w/ braces:**

    myFunction("lol",var);

**Declare w/ cleanliness:**

    myFunction "lol",var

### Declare a core procedure

**Declare w/ braces:**

    init MyProcedure {
        print("Hi")
    }

**Declare w/ cleanliness:**

    init MyProcedure
        print "Hi!"
