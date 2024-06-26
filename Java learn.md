### Switch statements 
```Java
import java.util.*; // import Scanner class
public class Main {
    public static void main(String[] args) {
        int a, b;
        Scanner input = new Scanner(System.in);
        System.out.println("Enter First Number: ");
        a = input.nextInt();
        System.out.println("Enter Second Number: ");
        b = input.nextInt();
        char c;
        System.out.println("Enter the operator +, -, *, /, or % : ");
        c = input.next().charAt(0);

        // switch statements
        switch (c) {
            case '+':
            System.out.println(a + " + " + b + " = " + (a + b));
            break;
            case '-':
            System.out.println(a + " - " + b + " = " + (a - b));
            break;
            case '*':
            System.out.println(a + " * " + b + " = " + (a * b));
            break;
            case '/':
            System.out.println(a + " % " + b + " = " + (a % b));
            break;
            case '%':
            System.out.println(a + " % " + b + " = " + (a % b));
            break;
            default:
            System.out.println("You have entered incorrect operator!");
        }
    }
}
```
### While Loop Examples
```Java
public class Main {
    public static void main(String[] args) {
        int i = 3;

        while (i > 0) {
            System.out.println(i);
            i--;
        }
        System.out.println("Happy New Year!");
    }
}
```
<p>While loop combined with an if else statement, let's say we play game of Yatzy:</p>

```Java
public class Main {
    public static void main(String[] args) {
        int dice = 1;

        while (dice <= 6) {
            if (dice < 6) {
                System.out.println("No Yatzy.");
            } else {
                System.out.println("Yatzy!");
            }
            dice = dice + 1;
        }
    }
}
```
### For Loop Examples
```Java
public class Main {
    public static void main(String[] args) {
        
        for (int i = 0; i <= 100; i += 10) {
            System.out.println(i);
        }
    }
}
```
```Java
public class Main {
    public static void main(String[] args) {
        
        for (int i = 0; i <= 10; i = i + 2) {
            System.out.println(i);
        }
    }
}
```
```Java
public class Main {
    public static void main(String[] args) {
        int n = 10;

        for (int i = 1; i <= n; i++) {
            System.out.println(i + " x " + n + " = " + (i * n) );
        }
    }
}
```
### Java methods
```Java
public class Main {
    public static void main(String[] args) {
        Main t1 = new Main();
        Main.gmail_method();
        System.out.println("All methods excuted!..");
    }

    static void gmail_method() {
        Main t1 = new Main();
        t1.product_method();
        System.out.println("Index: 10 messages unread!");   // static to non static
    }

    void product_method() {
        Main t1 = new Main();
        t1.windows_method();
        System.out.println("Google products Apps most use android");    // non static to non static
    }

    void windows_method() {
        Main.spotify_method();
        System.out.println("Windows 11 update 11.4.201.001 installing");    // non static to static
    }

    static void spotify_method() {
        Main.college_method();
        System.out.println("Play On High On Love Song");    // static to static
    }

    static void college_method() {
        int a = 2024;
        String b = "recent graduates in ";
        System.out.println("I am Hariharan " + b + a + " completed."); 
    }
}
```
### Output
```
I am Hariharan recent graduates in 2024 completed.
Play On High On Love Song
Windows 11 update 11.4.201.001 installing
Google products Apps most use android
Index: 10 messages unread!
All methods excuted!..
```
### Java method parameters
<p>Parameters and arguments</p>
<p>Java return methods</p>

```Java
public class Main {
    public static void main(String[] args) {
        Main t1 = new Main();
        Main.gmail_method();
        t1.product_method();
        String google = t1.product_method();
        System.out.println(google);
        Main.windows_method("11.4.201.001");
        
        String student = t1.college_method(2024);
        System.out.println("I am Hariharan " + student + " completed.");
    }

    static void gmail_method() {
        System.out.println("Index: 10 messages unread!");   // no return, no arguments
    }
    
    String product_method() {
        return "Google products Apps most use android";   // with return, no arguments   
    }

    static void windows_method(String a) {
        System.out.println("Windows 11 update " + a + " Installing");   // no return, with arguments
    }

    String college_method(int a) {
        String b = "recent graduates in " + a;   // with return, with arguments
        return b;   // added return statement
    }
}
```
