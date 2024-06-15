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