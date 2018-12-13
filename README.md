# Algorithmics

A Java library for people who want to implement some algorithms quickly.

**List of Current Algorithmics' Classes**
- SievePrimesAlgorithm

  >Find and Generate Prime numbers using Sieve's algorithm.
  
- NumOccurencesOfCharacters

  >Find number of occurences of different/particular character(s) in a string.
  
- Divisors

  >Find number of divisors of the number of your choice.
  
- CheckPrime

  >Check if a number is prime or not, efficiently.
  
- GetDivSquareSum

  >Get sum of squares of divisors of a number efficiently.
  
- BinarySearch

  >Search result for a number in an array of integers.
  
- MaxSubArraySum

  >Find the maximum continuous sub array sum in a given array.
  
- FindMaxSubArrayProduct  
  >Find the maximum continuous sub array prodyct in a given array of fixed length and no length constraint.

***

# Docs

- **SievePrimesAlgorithm**

This class helps you to find if a number is prime or not, for number upto 1 million, within a millisecond. 

To use this library, just make an object of this class, and call method `start()` in the beginning of your program. After that, just use `isPrime()` method to find boolean value corresponding to the number which is prime or not.

```
public boolean isPrime(int number){
  // returns boolean value stating the number is prime or not
}
```

Example code, for understanding:
```
public static void main(String[] args){

  SievePrimesAlgorithm prime = new SievePrimesAlgorithm();
  prime.start();
  .
  .
  .
  System.out.printlnt(prime.isPrime(83478)); // returns false as the number is not prime
}
```

- **NumOccurencesOfCharacters**

This class helps you find number of characters in a String of your choice. You can find number of occurences of a character of your own choice or you can find number of occurences of all characters individually.

To use this library, simply make an object of this class, and call `findNumOccurencesOfCharacter( myString, myCharacter)` to find number of occurences of `myCharacter` in `myString`. You can also use the method `findNumOccurencesOfAllCharacters(myString)` to get number of occurences of all characters present in `myString`.

```
public int findNumOccurencesOfCharacter(String myString, char myCharacter){
  // returns int stating the number of occurences of myCharacter in myString
}
```

```
public void findNumOccurencesOfAllCharacters(String myString){
  // prints number of occurences of each character
}
```

Example code, for understanding

```
public static void main(String[] args){

    NumOccurencesOfCharacters nm = new NumOccurencesOfCharacters();
		
		nm.findNumOccurencesOfAllCharacters("hehehe"); // prints number for each character
		
		System.out.println(nm.findNumOccurencesOfCharacter("abcadefgh", 'a' )); // prints 2
    
}
```

- **Divisors**

This class finds all the divisors of the number of your choice in O(n) time, the time complexity will soon be decreased even furthur.

To use this class, just make a simple object of `Divisors` class and call `findDivisors()` method which returns you an `ArrayList<Integer>` which contains all the divisors of the number in ascending order.

```
public ArrayList<Integer> findDivisors(int number){
	// returns ArrayList of all the divisors of the number sorted in ascending order
}
```

Example code, for understanding:

```
public static void main(String[] args){

     Divisors d = new Divisors();
		
     System.out.println(d.findDivisors(10)); // returns [1,2,5,10]
    
}
```

- **CheckPrime**

Sometimes using Sieve's algorithm is much more redundant and we need a quick and even more efficient solution for checking if a number is Prime or not. This is the reason of existence of this class.

To use this class, just make a simple object of `CheckPrime` class and call `checkPrime()` method which returns you an `boolean` value corresponding to the number.

```
public boolean checkPrime(long number){
	// returns true if the number is prime, otherwise fase
}
```

Example code, for understanding:

```
public static void main(String[] args){

    CheckPrime cp = new CheckPrime();
    
    System.out.println(cp.checkPrime(999999937)); // gives true as this is the largest 9 digit prime number
    
}
```

- **GetDivSquareSum**

Getting the sum of squares of divisors of a number is getting too much common in many competetive programming problems, and this becomes a tedious task to do in complexity less than O(n). This is why, this class exists.

To use this class, just make a simple object of `GetDivSquareSum` class and call `sumDivSquare()` method which returns you an `long` value corresponding to the sum of the square of the divisors of the number of your choice.

```
public long sumDivSquare(int num){
	// returns sum of squares of the divisors of the num
}
```

Example code, for understanding:

```
public static void main(String[] args){

    GetDivSquareSum gd = new GetDivSquareSum();
    
    System.out.println(gd.sumDivSquare(42)); // prints 2500 that is sum of squares of the divisors of 42
    
}
```

- **BinarySearch**

Searching for a particular number's existence in an array has always been one of the most widely used and fundamental part of any coding algorithm for a problem. BinarySearch has always been the most preferred one, so now use BinarySearch without coding the whole algorithm.

To use this class, just make a simple object of `BinarySearch(int[] array)` class and call `search()` method which returns you the boolean value stating the value exists in the array or not.

```
public boolean search(int num){
	// returns true or false depending on the existence of the number in the array
}
```

Example code, for understanding:

```
public static void main(String[] args){

	int[] arr = {1,5,3,14,2,12,7,6};
		
	BinarySearch b = new BinarySearch(arr);
		
	System.out.println(b.search(5)); // returns true
    
}
```

- **MaxSubArraySum**

Searching for a maximum sum of continuous sub-arrays in a given array is fastly becoming one of the most used and favorite algorithm in coding competitions and interview problems. You may often find it tedious to code this efficiently, hence this class to help you out.

To use this class, just make a simple object of `MaxSubArraySum(int[] array)` class and call `getSum()` method which returns you the int value (taking into account for positive and negative numbers) corresponding to the maximum sum of subarrays in your given array.

```
public boolean getSum(){
	// returns maximum continuous sub-array sum for your desired array
}
```

Example code, for understanding:

```
public static void main(String[] args){

	int[] arr = {1,-2,3,-2,5};
		
	MaxSubArraySum max = new MaxSubArraySum(arr);
		
	System.out.println(max.getSum()); // returns 6, that is sum of {3,-2,5}
    
}
```

- **FindMaxSubArrayProduct**

Searching for a maximum product of continuous elements of an array is also very common in coding problems and many complex alogrithms. There is also need for getting `k` elements max sub array product in an array. Hence this class, which finds you the desired product efficiently.

To use this class, just make a simple object of `FindMaxSubArrayProduct(int[] array)` class and call `findMaxProduct()` method which returns you the max sub array product for the whole array.

```
public boolean findMaxProduct(){
	// returns maximum continuous sub-array product for your desired array
}
```

There is also another method which lets you find maximum product of `k` element subarrays in your array. It's structure looks like this:

```
public boolean findMaxProduct(int k){
	// returns maximum continuous sub-array of length k product for your desired array
}
```

Example code, for understanding:

```
public static void main(String[] args){

	int[] arr = {1,-2,3,-2,5};
		
	FindMaxSubArrayProduct fm = new FindMaxSubArrayProduct(arr);
		
	System.out.println(fm.findMaxProduct(2)); // returns -2 that is product of length 2 sub array {1,-2}
		
	System.out.println(fm.findMaxProduct()); // returns 15 that is max product possible for your array
    
}
```

**New additions will be on roll, keep a look out :)**
  
  
