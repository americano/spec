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

**Note:** `int` isn't neccesarily needed, as it is assumed for any non-decimal number.
	
### Float
Decimal number

	float floatvarthingy = 3.5
	
**Note:** `float` isn't neccesarily needed, as it is assumed for any decimal number.

### String
An alphanumerical string, wrapped in phrase marks.

	str stringvarthingy = "Stringy Thingy" 
    
**Note:** `str` isn't neccesarily needed, as it is assumed, based on "".
	
### Array
A basic array.

	arr arrayvarthingy = [1,"Test",3,4,5]
	
The array isn't singularly typed: an array can hold multiple data types.

**Note:** `arr` isn't neccesarily needed, as it is assumed, based on [].

## Functions and Core procedures

### Declare a function
A basic function.

**Declare w/ braces:**

    func myFunction(s,var){
    	print("Hi");
    	return s;
    }


**Declare w/ cleanliness:**

    func myFunction(lol, var)
    	print("Hi")
    	return s

**Note:** `func` isn't neccesarily needed, as it is assumed, based on name and brackets.

### Execute a function
Run a function

**Declare w/ braces**

    x = foo(y);

**Declare w/ cleanliness**

    x = foo(y)

### Declare a core procedure

**Declare w/ braces:**

    init procedure {
        print("Hi")
    }

**Declare w/ cleanliness:**

    init procedure
        print("Hi!")

## Preprocessing

While Americano itself is a preprocessor, the language contains a unique two-layer preprocessing system, designed for making Americano remain an incredibly flexible language, despite not having an integreated processor-linked compiler.

### Layer 1

The first preprocessing layer is actually your normal code, nothing to note about this...

### Layer 2

Layer 2 is parsed _just-before-native-compiling_, taking advantage of the ability to know processor, OS, and other device unique data. This collects the data during native compilation.

This is done via a primitive syntax with indents.
**Note:** Use ">" to write to final script.

Eg.:

	#if os.type = "win"
    #	> print "Your OS is rubbish"
    #elseif os.type = "nix"
    #	> print "Hurray! Nix."
    #else
    #	> print "Compiler is clueless. :( \n At least you aren't using windows."

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