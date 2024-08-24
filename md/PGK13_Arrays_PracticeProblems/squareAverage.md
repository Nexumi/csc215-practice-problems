# [Managing and manipulating array contents](../)

> By: Jimmy Pan

<hr>

- Problem 1: Create a method that takes in an array and squares each element in the array.
- Problem 2: Create a method that takes the array from Problem 1, and calculate the average.

```java
import java.util.Arrays;
```
```java
// Problem 1 Test Case
int[] array = {7, 1, 4, 9, 18, 72, 36, 65};
squareUp(array);
System.out.println(Arrays.toString(array)); // [49, 1, 16, 81, 324, 5184, 1296, 4225]

// Problem 2 Test Case
System.out.println(average(array)); // 1397
```