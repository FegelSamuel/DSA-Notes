# Analysis of Algorithms
## Running Time
* Straightforward, just how long your program or function runs physically
* There is a **best**, **average**, and **worst** case.
```java
long startTime = System.currentTimeMillis();
/* insert algorithm here */
long endTime = System.currentTimeMillis();
long elapsed = endTime - startTime;
```
## Random Access Memory
* Really old model and still works
* Consists of a CPU
* Potentially unbounded bank of memory cells that hold an arbitrary number or char
* Memory cells are numbered and accessing any cell in memory takes unit time, however this is not sequential, so it's much faster than Disk Memory
## Functions of Time Complexity
| Name     | Function|
| -------- | ------- |
| Constant  | 1  |
| Logarithmic | log(n)     |
| Linear   | n    |
|N-Log-N | nlog(n) |
| Quadratic | n^2 |
| Exponential | 2^n |
| Factorial | n! |
log roots don't matter
## Primitive Operations
Operations that take Constant time like `if (x == 5) { print("haha"); }`
* __Important Note: Time Complexity follows the rules of limits__
* 3n^3 + 20n^2 + 5 = O(n^3)
