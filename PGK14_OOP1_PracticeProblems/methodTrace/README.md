# [Tracing Method Calls](../)

> By: Jimmy Pan

<hr>

- What is the output of this code?

```java
import java.util.Arrays;
public class Main {
    public static int firstMethod(int[] arr, int x) {
        int z = 0;
        for (int i = 0; i < arr.length; i++) {
            z = z + arr[i] * x;
        }
        return z;
    }

    public static String secondMethod(int x, String str) {
        String s = "";
        for (int i = 0; i < x; i++) {
            s = s + str;
        }
        return s;
    }

    public static double[] thirdMethod(int x) {
        double[] arr = new double[x];
        for (int i = 0; i < x; i++) {
            arr[i] = x;
        }
        return arr;
    }

    public static void finalMethod(int x, String str, double[] arr) {
        System.out.printf("%d     %s     %s", x, str, Arrays.toString(arr));
    }

    public static void main(String[] args) {
        finalMethod(firstMethod(new int[]{5, 7, 35, 52}, 3), secondMethod(3, "xyz"), thirdMethod(5));
    }
}
```