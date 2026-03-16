## 1.Basic Array Syntax
### 1.0 some rules
- the ==type== of every object of an array must be the same, unlike python.
	- ***reference can also be a type***
- the ==length== of an array cannot be changed.
- the address of every array is 64-bit.
- the objects are ==anonymous==. Once you lose the reference, its gone forever.
	`int[] y = {1, 2}; y = new int[3];`
### 1.1 create an array
- default value
- `z = new int[0];` creates an empty array
- the parameter of length can be **omitted** if the array is instantiated once created.
### 1.2 instantiate an array
- calculations can be done automatically
	`s[s[1] - s[3]] = 5;` is legitimate
### 1.3 array copy
- `System.arraycopy(copy_array, start_copied_position, copy_to_array, start_position, length);`
- two references to the same array('=') vs ==none-destructive== operations
- *slice notations in python*
- copy goes faster than simply loop

# 2. 2-D Arrays
## 2.1 create a 2-D array
- `int[][] Array1;` `Array1 = new int[4][];` every array nested in Array1 don't have to have the same length.

# 3. Arrays vs Classes
- arrays cannot have methods
- access: bracket notation vs dot notation
- users can interact with arrays, while cannot with classes.
	`askUser();`
	*reflections API* (not recommended, but makes it possible to access things inside a class without **hard-coded dot notation**)