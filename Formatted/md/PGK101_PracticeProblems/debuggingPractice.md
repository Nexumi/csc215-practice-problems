# Debugging Practice

> By: Turk Erdin

- The code below is broken. I have placed the expected output in the comments. Using the debugger tool and everything you've learned about loops, go through and debug this faulty code so it prints as expected.

```
import java.util.*;

public class DebuggingPractice {
    public static void main(String[] arg) {
        Scanner sc = new Scanner(System.in);
        
        /**
           Expected output:
           
           How many layers in your pyramid do you want?
           4

           *
           * *
           * * *
           * * * *
         */
        System.out.println("How many layers in your pyramid do you want?");
        int levels = sc.nextInt();
        
        System.out.println();
        
        for (int i=0; i<=levels; i++) {
            for (int j=i-1; j>0; j++) {
                System.out.print("* ");
            }

            System.out.println();
        }

        /**
           Expected output:
           
           What is your name?
           Turk

           K R U T
         */
        System.out.println("What is your name?");
        String str = sc.nextLine().toUpperCase();
        String str2 = "";

        System.out.println();
        for (int i=str.length(); i<0; i--) {
            str2 += str.charAt(i);
        }

        System.out.println(str2);

        sc.close();
    }
}
```