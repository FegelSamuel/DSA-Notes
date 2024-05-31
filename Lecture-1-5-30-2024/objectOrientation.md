# Instructor Information (misc)
* Heavy industry experience
* Does grad and undergrad courses
* Random Quizzes, they are not graded but you need to do them
* There is a curve
# Recursion
## Find Factorial
```C
#include <iostream>
unsigned long long int factorial(unsigned long long int n) {
    if (n <= 1) {
        return 1;
    }
    else {
        return n * factorial(n - 1); // function is called n amount of times
    }
}

int main()
{
    // The time complexity to find the factorial of a given integer is O(n)
    std::cout << "Factorial of 4: " << factorial(64) << '\n';
    return 0;
}
```
## Binary Search
I stole this from [Geeks For Geeks](https://www.geeksforgeeks.org/cpp-binary-search/#). This runs in O(log(n)) time (root of logarithm doesn't matter, it could be ln for all we care)
```C
int binarySearch(int arr[], int low, int high, int x) // x is target
{ 
    // Base case: If the search space becomes empty, the element is not present in the array 
    if (high >= low) { 
        // Calculate the middle index to divide the search 
        // space in half 
        int mid = low + (high - low) / 2; 
  
        // If the middle element is equal to 'x', we have 
        // found the element, return its index 
        if (arr[mid] == x) 
            return mid; 
  
        // If the middle element is greater than 'x', search 
        // in the left half of the array 
        if (arr[mid] > x) { return binarySearch(arr, low, mid - 1, x); }
  
        // If the middle element is less than 'x', search in 
        // the right half of the array 
        return binarySearch(arr, mid + 1, high, x);
    }
    // If the base case is reached, the element is not present in the array, return -1 
    return -1; 
}
```
## Exponent
x^n
```C
int power(x, n) {
if (n = 0) { return 1; }
if (n % 2 == 1) { y = power(x, (n - 1)/2); return x * y * y; }
else { y = power(x, n/2); return y * y; }
```
## Tail Recursion
* Tail recursion happens when a linearly recursive method makes ts recursive call as its last step
## Binary recursion
* fib
