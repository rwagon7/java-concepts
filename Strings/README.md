# Strings

## public final class String extends Object implements Serializable, Comparable<String>, CharSequence, Constable, ConstantDesc

## Intialization
- String s = "abc";
- String s = { "a", "b", "c"};
- String s = new String(data);

## Constructor intialization
=> can bbe used with byte[] which gets converted into string
- String(byte[] bytes, Charset charset);
=> Constructs a new String by decoding the specified array of bytes using the specified charset.
- String(int[] codePoints, int offset, int count);
=> Initializes a newly created String object so that it represents the same sequence of characters as the argument; in other words, the newly created string is a copy of the argument string.
=> 
- String(StringBuffer buffer)
=> Allocates a new string that contains the sequence of characters currently contained in the string builder argument.
- String(StringBuilder builder)
=> Allocates a new string that contains the sequence of characters currently contained in the string builder argument.

## Methods   
--------------------------------------------------------------------------------------------------------------------------------------------------------
|   Modifier & types |  Methods                         | Description                                                                                  |
|--------------------|----------------------------------|----------------------------------------------------------------------------------------------|
|   char             |  charAt(int index)               |Returns the char value at the specified index.                                                |
|   int              |  codePointAt(int index)          |Returns the character (Unicode code point) at the specified index.                            |
|   int              |  codePointBefore(int index)      |Returns the character (Unicode code point) at the specified index.                            |
|   int              |  codePointAt(int index)          |Returns the character (Unicode code point) at the specified index.                            |
|   int              |  compareTo(String anotherString) |Compares two strings lexicographically.                                                       |
|   int              |  compareToIgnoreCase(String str) |Compares two strings lexicographically, ignoring case differences.                            |
|   String	         |  concat(String str)	            |Concatenates the specified string to the end of this string.                                  |
|   boolean	         |  contains(CharSequence s)	    |Returns true if and only if this string contains the specified sequence of char values.       |
|   boolean	         |  contentEquals(CharSequence cs)	|Compares this string to the specified CharSequence.                                           |
|   static String	 |  copyValueOf(char[] data)	    |Equivalent to valueOf(char[], int, int).                                                      |
|   boolean	         |  endsWith(String suffix)	        |Tests if this string ends with the specified suffix.                                          |
|   boolean	         |  equalsIgnoreCase(String s2)	    |Compares this String to another String, ignoring case considerations.                         |
|   static String    |  format(String f,Object... args) |Returns a formatted string using the specified format string and arguments.                   |
|   byte[]	         |  getBytes()	                    |Encodes into a sequence of bytes platform charset                                             |
|   int	             |  hashCode()	                    |Returns a hash code for this string.                                                          |
|   String	         |  indent(int n)	                |Adjusts the indentation of each line of this string based on the value of n.                  |
|   int	             |  indexOf(int ch)                 |Returns the index within this string of the first occurrence of the specified character.      |
|   String           |  intern()                        |Returns a canonical representation for the string object.                                     |
|   boolean	         |  isBlank()	                    |Returns true if the string is empty or contains only white space codepoints, otherwise false. |
|   boolean	         |  isEmpty()	                    |Returns true if, and only if, length() is 0.                                                  |
|  Stream<String>	 |  lines()	                        |Returns a stream of lines extracted from this string, separated by line terminators.          |
|  boolean	         |  matches(String regex)	        |Tells whether or not this string matches the given regular expression.                        |
|  String	         |  repeat(int count)	            |Returns a string whose value is the concatenation of this string repeated count times.        |
|  String	         |  replace(char old, char new)	    |Returns a string resulting from replacing all occurrences of oldChar in String to newChar.    |
|  String	         |  replaceAll(String rgx, String s)|Replaces each substring of this string that matches the given regular expression.             |
|  String	         |  substring(int beginIndex)	    |Returns a string that is a substring of this string.                                          |
|  char[]	         |  toCharArray()                   |Converts this string to a new character array.                                                |
|  String	         |  toLowerCase()	                |Converts all of the chars in this String to lower case using the rules of the default locale. |
|  <R> R	         |  transform(Function<?> f)	    |This method allows the application of a function to this string.                              |
|  String	         |  translateEscapes()	            |Returns a string, with escape sequences translated as if in a string literal.                 |
|  String	         |  trim()	                        |Returns a string whose value is this string, with all leading and trailing space removed      |
|  static String	 |  valueOf(Object obj)	            |Returns the string representation of the Object argument.                                     |
--------------------------------------------------------------------------------------------------------------------------------------------------------