# Java-Day-12-Smallest-of-Three-Numbers
# Java Day 12 - Smallest of Three Numbers

This program takes three numbers from the user and finds the smallest number using conditional statements.

## Example

Input:

```text
25
12
30
```

Output:

```text
Smallest number = 12
```

## Concepts Used

* Scanner
* User input
* Variables
* `if`
* `else if`
* `else`
* Comparison operators
* `&&` AND operator

## How It Works

1. The program creates a `Scanner` object to take user input.
2. The user enters three numbers.
3. The first number is compared with the other two numbers.
4. If the first number is the smallest, it is displayed.
5. Otherwise, the second number is checked.
6. If neither the first nor second number is the smallest, the third number is displayed.
7. The smallest number is printed on the screen.

## Java Code

```java
import java.util.Scanner;

public class Main
{
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter first number: ");
        int num1 = sc.nextInt();

        System.out.print("Enter second number: ");
        int num2 = sc.nextInt();

        System.out.print("Enter third number: ");
        int num3 = sc.nextInt();

        if (num1 <= num2 && num1 <= num3)
        {
            System.out.println("Smallest number = " + num1);
        }
        else if (num2 <= num1 && num2 <= num3)
        {
            System.out.println("Smallest number = " + num2);
        }
        else
        {
            System.out.println("Smallest number = " + num3);
        }

        sc.close();
    }
}
```

## Output

```text
Enter first number: 25
Enter second number: 12
Enter third number: 30
Smallest number = 12
```

## Goal

The goal of this project is to practice conditional statements, comparison operators, and the `&&` operator by finding the smallest of three numbers in Java.
