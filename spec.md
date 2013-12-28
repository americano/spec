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

    str func myFunction(str s, int var){
    	print("Hi");
    	return s;
    }


**Declare w/ cleanliness:**

    str func myFunction(str "lol", int var)
    	print("Hi")
    	return s

Note that the type declaration in-front of the function name is the type of variable returned, if none is written then `void` (a returnless function) is assumed. 
### Execute a function
Run a function

**Declare w/ braces**

    x = foo(y);

**Declare w/ cleanliness**

    x = foo(y)

### Declare a core procedure

**Declare w/ braces:**

    init MyProcedure {
        print("Hi")
    }

**Declare w/ cleanliness:**

    init MyProcedure
        print("Hi!")

## Preprocessing

While Americano itself is a preprocessor, the language contains a unique two-layer preprocessing system, designed for making Americano remain an incredibly flexible language, despite not having an integreated processor-linked compiler.

### Layer 1

The first preprocessing layer is actually your normal code, nothing to note about this...

### Layer 2

Layer 2 is parsed _just-before-native-compiling_, taking advantage of the ability to know processor, OS, and other device unique data. This collects the data during native compilation.

## Importing

To import an internal library(included with americano), do:

    import foo

**Or:**

    import("foo");
    
To import part of an internal library, do:

    import foo.bar

**Or:**

    import("foo.bar");

To access an internal library, but would like to use a different name, do:

    bar = import foo

**Or:**

    bar = import("foo");
