# [Generate Random Numbers](../)

> By: Jimmy Pan

<hr>

- Create a method that generates a random String of length 6, using only 0-9 and a-f, then add `0x` in front of it. Also generate a random number from 1 to 16777215.
    - Please use the given main method and do not make any modifications to it.
    - Fun fact: `0xfa12ce` is what we call a hexadecimal number.

```java
public static void main(String[] args) {
    Object[] numbers = generateRandomNumbers();
    String hex = (String) numbers[0];
    int dec = (int) numbers[1];
    System.out.printf("Random Hexadecimal Number: %s%n", hex);
    System.out.printf("Random Decimal Number: %d%n", dec);
}
```