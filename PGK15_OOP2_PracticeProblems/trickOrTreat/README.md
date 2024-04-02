# [(Trick or Treat) and Trace!](../)

> By: Jimmy Pan

<hr>

- Figure out the output of this code without the use of an IDE.

```java
public class Main {
    public static void main(String[] args) {
        Halloween you = new Halloween();
        you.buyCandy(50);
        for (int i = 1; i <= 5; i++) {
            you.giveCandy(i * ((i % 2 == 0) ? 3 : 4));
        }
        System.out.printf("I end the night with %d piece(s) of candy.%n", you.getCandy());
    }
}

public class Halloween {
    private int candy;

    public Halloween() {
        this.candy = 0;
    }

    public Halloween(int candy) {
        this.candy = candy;
    }

    public int getCandy() {
        return this.candy;
    }

    public int buyCandy(int amount) {
        if (amount < 0) {
            System.out.println("Silly you, you can't buy negative pieces of candy :)");
        } else {
            System.out.printf("You went out and bought %d piece(s) of candy.%n", amount);
            this.candy = this.candy + amount;
        }

        return this.candy;
    }

    public int giveCandy(int amount) {
        if (amount < 0) {
            System.out.println("Silly you, you can't give negative pieces of candy :)");
        } else {
            System.out.printf("You gave out %d piece(s) of candy.%n", amount);
            this.candy = this.candy - amount;
        }

        return this.candy;
    }

    public void trickOrTreat(boolean treat) {
        if (treat) {
            System.out.printf("Here are %d pieces of candy!%n", 5);

        } else {
            System.out.printf("You have been tricked and had %d pieces of candy stolen from you :(%n", 2);
        }
    }
}
```