Download Link: https://assignmentchef.com/product/solved-homework-03
<br>
<p class="ui header product-top-header" title="HW03 Solution">Objective

The purpose of this assignment is to add overloading operators and I/O streams.

Project Description

In the last assignment, we wrote a basic String class. This time, you must enhance your old String class that now provides some other basic String operations. Your new String class should update or provide the following methods in the String class for setting up, accessing and changing strings (overloading operators (2) to (7) internally and (9) externally):

(1) Add a new constructor that initializes the String object by a string s.String(const char s[]);

(2) String operator +=(const String &amp;str); // formerly void append(const String &amp;str);Overload += operator. A method that returns a string formed by appending the passed String with the String the method is called on,

(3) char operator [](int i) const; // formerly char element(int i) const;Overload operator [] A method that returns the ith element (zero-based, just like arrays) of the String it is called on. This method  should print out an error message and return the null character ( ) if the location asked for is out-of-range for the string.

(4) bool operator ==(const String &amp;str) const;

Note: you can use the library functions provided by .  For example, this is an implementation of overloading operator == :

(5) bool operator !=(const String &amp;str) const;(6) bool operator (const String &amp;str) const;(7) bool operator &lt;(const String &amp;str) const;// all of them are formerly int compare_to(const String &amp;str) const; that compares the String object with the String passed to this method. Each returns a true or false value based on whether the relationship (e.g., ==, !=, , &lt;, =, &lt;=) holds or not.

(8) void print(ostream &amp;out) const; //formerly void print() const; which only prints to standard output screenA method that prints the value of the String it is called on to ostream object out.

(9) ostream &amp; operator &lt;&lt; (ostream &amp;out, const String &amp; r);An external overloading output stream operators &lt;&lt; by calling methods (8) as in the example of Time class (refer text page 171-172.

Note: In your implementation of String’s methods, you may use the library functions provided by , which operate on the C style string. Our textbook contains good review about it  page 212 to 214, and Appendix D 5.

Download Test Driver: We provide a driver (file Assign3_2driver.cpp ) that you can download and use to test your new class. You are not allowed to change it!