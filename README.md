# CST126_01 - Plastic spoons and strings

Class ID: Vulpix

Assignement ID: CST126_01

Unresolved Issues: None.

Notes: A full set of the main code runs from line 10 to approx line 23 (with a delete function). The reason all delete
functions are at the very end is because my code would just stop working if I had a delete[] ptr before I would run everything
again for the empty string.

Pleasen note: I tried creating my own strlen function. However, I ran into a few problems imitating the "What came first:
chicken or egg issue." In order to create a dynamic array using new and assigning to a pointer, I had to give it a size. In order
to give it a size, I had to make my own strlen function. But in order to make the strlen function, I needed an array in order
to use its pointer to check for the null character (to figure out the total size). But in order for an array, I needed a dynamic array.
Therefore, I used the sizeof for a variable that I had utilized in the dynamic array. 

Thank you for the assigment and for the extension. I had learned a lot.


---

**Purpose:**  
	Practice working with pointers  
	Practice working with the heap  

**Goal:**

  Create a string function that identifies the location of a character within a string.  The FIND function 
  should locate character within a text string, and return the number of first location of the character 
  within the text string.  
	
	Your program has the following restrictions.  

	  - The text function should take a pointer to a char for the string.  
	  - You may not use any string functions or cstring functions.  If you need these functions, 
	    you should write them yourself.  
	  -   You may only use pointers / pointer arithmetic to access your strings
			(hint:  I wrote my own strlen and strcopy functions using pointer arithmetic.)
	  - The FIND function should be case sensative.
	  - Your FIND function should return a -1 if the character isn't found.
	  - Your FIND function should handle an empty string. 
	  - Use human indexed format not C++ indexing.  So the first character is position 1.
	  - You clean your heap up before you exit the program.  No memory leaks.

---

Output Format  
=============

\-\- _input string_ \-\-    
_char_ is in position nn  

Testing Data  
=============
Run your program with the following test data:

**String:**  "I was born with a plastic spoon in my mouth."  
**Characters:**  i, I, w, z, r     

**String:**  ""  
**Character:** y  

Sample Output
=============

Given the test set above, the output would be:

-----

\-\- I was born with a plastic spoon in my mouth. \-\-  
i is in position 13  
I is in position 1  
w is in position 3  
z is in position -1  
r is in position 9  

\-\-  \-\-  
y is in position -1    
