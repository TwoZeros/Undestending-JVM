# Задача "Понимание JVM"

## Цель работы
Описать текстом и/или картинками каждую строку исходного кода программы на языке JAVA с точки зрения происходящего в JVM  


## Код для исследования
```java
public class JvmComprehension {
    public static void main(String[] args) {
        int i = 1;                      // 1
        Object o = new Object();        // 2
        Integer ii = 2;                 // 3
        printAll(o, i, ii);             // 4
        System.out.println("finished"); // 7
    }
    private static void printAll(Object o, int i, Integer ii) {
        Integer uselessVar = 700;                   // 5
        System.out.println(o.toString() + i + ii);  // 6
    }
}

##  Ход работы
