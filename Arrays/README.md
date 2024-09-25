# Arrays

## asList
- returns static List<T> by taking input T[]

## binarySearch
- Searches the specified array of bytes for the specified value using the binary search algorithm. returns statuc int
- This method is overloaded
- Arrays.binarySearch(byte[] a, byte[] key)
- Arrays.binarySearch(byte[] a, char key);
- Arrays.binarySearch(byte[] a, int fromIndex, int toIndex, byte key);
- Arrays.binarySearch(byte[] a, int fromIndex, int toIndex, char key);
- Arrays.binarySearch(byte[] a, double key);
- Arrays.binarySearch(byte[] a, float key);
- Arrays.binarySearch(byte[] a, int fromIndex, int toIndex, float key);
- Arrays.binarySearch(byte[] a, int fromIndex, int toIndex, double key);
- Arrays.binarySearch(byte[] a, int key);
- Arrays.binarySearch(byte[] a, long key);
- Arrays.binarySearch(byte[] a, int fromIndex, int toIndex, long key);
- Arrays.binarySearch(byte[] a, short key);
- Arrays.binarySearch(byte[] a, int fromIndex, int toIndex, short key);
- Arrays.binarySearch(T[] a, int fromIndex, int toIndex, T key, Comparator<? super T> c);
- Arrays.binarySearch(T[] a, T key, Comparator<? super T> c);

... And many more

## compare
- works only with this modifiier static <T extends Comparable<? super T>>
- This method is overloaded
- Compares two Object arrays, within comparable elements, lexicographically. => compare(T[] a, T[] b);
- Compares two Object arrays lexicographically using a specified comparator. => compare(T[] a, T[] b, Comparator<? super T> cmp);


## copyOf
- This works with static int[] modifier
- Copies the specified array, truncating or padding with zeros (if necessary) so the copy has the specified length.
 => Arrays.copyOf(int[] original, int newLength).
- Copies the specified array, truncating or padding with nulls (if necessary) so the copy has the specified length.
 => Arrays.copyOf(U[] original, int newLength, Class<? extends T[]> newType)
- Copies the specified range of the specified array into a new array.
 => Arrays.copyOfRange(T[] original, int from, int to)

## deepEquals, equals, deepHashCode & deepToString
- deepEquals(Object[] a1, Object[] a2).
=> Returns true if the two specified arrays are deeply equal to one another.
- equals(boolean[] a, boolean[] a2)
=> Returns true if the two specified arrays of booleans are equal to one another.
-  deepHashCode(Object[] a)
=> returns a hashcode based on deep contents
- deepToString(Object[] a)
=> Returns a string representation of the "deep contents" of the specified array.
- equals(boolean[] a, int aFromIndex, int aToIndex, boolean[] b, int bFromIndex, int bToIndex)
=> This method is overloaded. Returns true if the two specified arrays of booleans, over the specified ranges, are equal to one another.

## fill
- fill(int i)
=> fills the each and every element of array with a deafult value.

## hashCode
- hashCode(int[] a)
=> Returns a hash code based on the contents of the specified array.

## mismatch
- 	mismatch(boolean[] a, boolean[] b)
=> This method is overloaded. Finds and returns the index of the first mismatch between two boolean arrays, otherwise return -1 if no mismatch is found.

## parllelsort
- this method is overloaded
- Sorts the specified array into ascending numerical order
=> parallelSort(byte[] a)
- Sorts the specified range of the array into ascending numerical order.
=> parallelSort(double[] a, int fromIndex, int toIndex)

## setAll
- setAll(double[] array, IntToDoubleFunction generator)
=> Set all elements of the specified array, using the provided generator function to compute each element.


## sort
- sort(int[] a)
=> Sorts the specified range of the array into ascending order

## Stream
- stream(T[] a)
=> converts array into streams
