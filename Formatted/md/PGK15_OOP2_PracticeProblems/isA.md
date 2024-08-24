# IS-A

> By: Jimmy Pan

- Figure out the output of this code without the use of an IDE.

```java
public class Main {
    public static void main(String[] args) {
        A a = new A();
        B b = new B();
        A ab = new B();
        B ba = (B) ab;

        a.one();
        a.two();
        b.one();
        b.two();
        ab.one();
        ab.two();
        ba.one();
        ba.two();
    }
}

class A {
    public A() {
    }

    public void one() {
        System.out.println("I am a statement.");
    }

    public void two() {
        System.out.println("I am another statement.");
    }
}

class B extends A {
    public B() {
    }

    @Override
    public void one() {
        System.out.println("I am one more statement.");
    }
}
```