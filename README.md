# Numbered Square Pattern Program

## Overview
The **Numbered_Square** program generates a square number pattern based on user input. The user specifies a size (**n**), and the program prints an **n × n** grid where each row consists of the same number, starting from **1** and increasing by **1** in each subsequent row.

## Code Implementation
```java
package number_patterns;

import java.util.Scanner;

public class Numbered_Square
{
    public static void main(String[] args)
    {
        Scanner s = new Scanner(System.in);
        System.out.println("Enter the size");
        int n = s.nextInt();
        int num = 1;
        
        for(int i = 1; i <= n; i++)
        {
            for(int j = 1; j <= n; j++)
            {
                System.out.print(num + " ");
            }
            System.out.println();
            num++;
        }
    }
}
```

---

## Explanation of the Code

### 1. **Importing the Scanner Class**
```java
import java.util.Scanner;
```
- The **Scanner** class is part of the `java.util` package and is used to take user input.
- It allows us to read different types of input, like integers and strings, from the console.

### 2. **Creating a Scanner Object**
```java
Scanner s = new Scanner(System.in);
```
- `Scanner s` is an object used to read user input.
- `System.in` allows input to be read from the keyboard.
- The scanner helps in reading the integer value entered by the user.

### 3. **Declaring Variables**
```java
int n = s.nextInt();
int num = 1;
```
- `n`: Stores the user-input integer which represents the size of the square.
- `num`: Keeps track of the number to be printed in each row, starting from **1**.

### 4. **Outer Loop (For Loop - Rows Control)**
```java
for(int i = 1; i <= n; i++)
```
- This loop runs **n** times, representing **n** rows in the pattern.
- The loop starts with `i = 1` and increments up to `n`, ensuring the required number of rows is printed.

### 5. **Inner Loop (For Loop - Columns Control)**
```java
for(int j = 1; j <= n; j++)
```
- This nested loop runs **n** times for each row.
- It prints the same number **n** times in a row.
- The value of `num` remains constant within a row but increments after each row.

### 6. **Printing Statements**
```java
System.out.print(num + " ");
```
- Prints the value of `num` followed by a space, ensuring proper formatting of the pattern.
- Uses `print()` instead of `println()` to keep numbers on the same line.

```java
System.out.println();
```
- Moves to the next line after printing **n** numbers, ensuring row-wise formatting.

### 7. **Incrementing the Number**
```java
num++;
```
- Increments the value of `num` after each row to print the next number in the following row.

---

## Example Execution
### **Input:**
```
Enter the size
4
```
### **Output:**
```
1 1 1 1
2 2 2 2
3 3 3 3
4 4 4 4
```

## Key Concepts Used
- **Java Basics**: Variables, Loops, User Input
- **Scanner Class**: Reading user input
- **For Loop**: Handling iteration over rows and columns
- **Printing Statements**: Managing console output formatting

## Use Cases
- Understanding nested loops.
- Practicing pattern printing problems.
- Strengthening knowledge of Java syntax.

## Conclusion
This program demonstrates a simple number pattern using loops and user input. It is useful for beginners to understand **nested loops**, **input handling**, and **formatted output** in Java.

## Clone
```
git clone https://github.com/Ananthadatta02/Java-Numbered_Square.git
```
