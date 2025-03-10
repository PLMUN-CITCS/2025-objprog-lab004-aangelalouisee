# **2025-OBJPROG-LAB004**
Week 02 - Introduction to Java Programming

Laboratory # 04 - Guided Coding Exercise: Arithmetic Operators and Operator Precedence

## **Instructions**

### **Step 1.1: Accept the Assignment**

   1. Click on the assignment link provided by your instructor.
   2. GitHub Classroom will create a **private repository** under your GitHub account.
   3. After the repository is created, click **"Go to Repository"** to view your assignment.

---

### **Step 1.2: Setup your Git Environment**
Only perform this if this is the first time you will setup your Git Environment

   1. Create a GitHub Account:
   ```bash
   https://github.com/signup?source=login
   ```
      
   2. Download and Install Git on your Laptop/Desktop:
   ```bash
   https://git-scm.com/downloads
   ```
   
   3. Create a Folder in your Laptop/Desktop
   4. Right-click anywhere in the created folder and select "Open Git Bash Here".
   5. In the Git Bash Terminal, set your git name, perform command:
   ```bash
   git config --global user.name "Your Name"
   ```
   
   6. In the Git Bash Terminal, set your git email, perform command:
   ```bash
   git config --global user.email "your.email@example.com"
   ```
   
   7. Create your SSH Key, just follow the instructions, no need to provide filename and passphrase. In the Git Bash Terminal, perform command:
   ```bash
   ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
   ```
   
   8. Copy your SSH Keys into clipboard. In the Git Bash Terminal, perform command:
   ```bash
   clip < ~/.ssh/id_rsa.pub
   ```
   
   9. Log in to your GitHub account.
   10. In the upper-right corner of GitHub, click your profile picture and select Settings.
   11. In the left sidebar, click on SSH and GPG keys.
   12. Click the New SSH key button.
   13. In the Title field, give the key a recognizable name (e.g., "My Windows Laptop").
   14. In the Key field, CTRL + V or paste the keys copied into your clipboard. Save the key.
   15. Go Back to terminal, use command:
   ```bash
   ssh -T git@github.com
   ```

### **Step 2: Clone the Repository to Your Local Machine**

   1. On your repository page, click the green **"Code"** button.
   2. Copy the repository URL (choose HTTPS for simplicity).
   3. Open your terminal (or Git Bash, Command Prompt, or PowerShell) and run:
   
   ```bash
   git clone <git_repo_url>
   ```
   
   4. Navigate into the cloned folder:
   
   ```bash
   cd <git_cloned_folder>
   ```

### **Step 3: Complete the Assignment**

**Laboratory # 04 - Guided Coding Exercise: Arithmetic Operators and Operator Precedence**

   **Objective:**
   - Apply arithmetic operators in Java.
   - Understand operator precedence with step-by-step calculation.

   **Desired Output:**
   ```txt
   Sum: 15
   Difference: 5
   Product: 50
   Quotient: 2
   Remainder: 0
   Expression Result: 18
   ```

   **File Naming Convention:**
   - `ArithmeticDemo.java`

   **Notable Observations (to be discussed after completing the exercise):**
   - Arithmetic Operators: The activity provides hands-on practice with the basic arithmetic operators: + (addition), - (subtraction), * (multiplication), / (division), and % (modulus).
   - Operator Precedence: The key observation is the demonstration of operator precedence. The example expression (num1 + num2 * 2 - (num1 / num2)) forces students to think about the order in which operations are performed.
   - Integer vs. Double: The activity uses integers for most calculations, but it also introduces a double. This is a good opportunity to discuss the difference between integer and floating-point arithmetic.
   - Modulus Operator: The inclusion of the modulus operator is important, as it's a commonly used operator that students might not be as familiar with as the others.
   - Step-by-Step Calculation: The instructions implicitly encourage students to perform a step-by-step calculation of the example expression to understand how operator precedence works. This is a valuable learning process.

   **Java Best Practices**
   - Declare Variables Before Use: Always declare your variables (int num1, int sum, etc.) before you try to use them.
   - Initialize Variables: It's good practice to initialize variables when you declare them (e.g., int num1 = 10;). This prevents potential issues with uninitialized variables.
   - Use Meaningful Variable Names: Use names that describe the purpose of the variable (e.g., sum, difference, product).
   - Understand Operator Precedence: Java follows standard operator precedence rules (like PEMDAS/BODMAS). Multiplication and division happen before addition and subtraction. Use parentheses () to enforce a specific order of operations if needed. This is very important for getting the correct results.
   - Integer Division: Be aware that integer division truncates (discards) the decimal part. If you need a more precise result, use double or float data types.
   - Modulus Operator: The modulus operator (%) gives you the remainder of a division. It's useful in many situations (e.g., checking if a number is even or odd).
   - Comments for Complex Expressions: If you have a complex expression, add a comment to explain the order of operations. This makes your code easier to understand.
   - Output with Labels: When you print results, always include clear labels to identify what each value represents (e.g., "Sum: " + sum). This makes the output much more user-friendly.
   
   **Step-by-Step Instructions:**

   1. Class and Main Method
      - Create a file named `ArithmeticDemo.java`.
      - Define the class `ArithmeticDemo` and its main method.
      ```Java
      public class ArithmeticDemo {
          public static void main(String[] args) {
      
          }
      }
      ```
      
   2. Declare and Initialize Integer Variables
      - Inside the `main` method, declare two integer variables, `num1` and `num2`.
      - Initialize `num1` with the value 10.
      - Initialize `num2` with the value 5.
      ```Java
      int num1 = 10;
      int num2 = 5;
      ```
            
   3. Declare and Initialize a Double Variable
      - Declare a double variable named `num3`.
      - Initialize `num3` with the value 3.0.
      ```Java
      double num3 = 3.0;
      ```

   4. Perform Addition
      - Declare an integer variable named `sum`.
      - Calculate the sum of `num1` and `num2` and store the result in `sum`.
      ```Java
      int sum = num1 + num2;
      ```

   5. Perform Subtraction
      - Declare an integer variable named `difference`.
      - Calculate the difference between `num1` and `num2` and store the result in `difference`.
      ```Java
      int difference = num1 - num2;
      ```

   6. Perform Multiplication
      - Declare an integer variable named `product`.
      - Calculate the product of `num1` and `num2` and store the result in `product`.
      ```Java
      int product = num1 * num2;
      ```

   7. Perform Integer Division
      - Declare an integer variable named `quotient`.
      - Calculate the integer division of `num1` by `num2` and store the result in `quotient`.  (Remember, integer division truncates any decimal part).
      ```Java
      int quotient = num1 / num2;
      ```

   8. Perform Modulus Operation
      - Declare an integer variable named `remainder`.
      - Calculate the remainder of the division of `num1` by `num2` (using the modulus operator `%`) and store the result in `remainder`.
      ```Java
      int remainder = num1 % num2;
      ```

   9. Demonstrate Operator Precedence
      - Declare an integer variable named `expressionResult`.
      - Calculate the result of the following expression and store it in `expressionResult: num1 + num2 * 2 - (num1 / num2)`.  Pay attention to the order of operations (multiplication and division before addition and subtraction). The parentheses enforce the division to happen first.
      ```Java
      int expressionResult = num1 + num2 * 2 - (num1 / num2);
      ```

   10. Output the Results
       - Use `System.out.println()` to print the value of `sum` with a descriptive label (e.g., "Sum: ").
       - Do the same for `difference`, `product`, `quotient`, `remainder`, and `expressionResult`.  Make sure each output has a clear label.  For the expressionResult, explain the order of operations used in the calculation in a comment.
       
```Java
System.out.println("Sum: " + sum);
System.out.println("Difference: " + difference);
System.out.println("Product: " + product);
System.out.println("Quotient: " + quotient);
System.out.println("Remainder: " + remainder);
System.out.println("Expression Result: " + expressionResult); // Explain order of operations
```

   11. Compile and Run
       - Save the file as `ArithmeticDemo.java`.
       - Compile the code using `javac ArithmeticDemo.java` in your terminal or command prompt.
       - Run the compiled code using `java ArithmeticDemo`.

### **Step 4: Push Changes to GitHub**
Once you've completed your changes, follow these steps to upload your work to your GitHub repository.

1. Check the status of your changes:
   Open the terminal and run:
   
   ```bash
   git status
   ```
   This command shows any modified or new files.
   
2. Stage the changes:
   Add all modified files to staging:
   
   ```bash
   git add .
   ```
   
3. Commit your changes:
   Write a meaningful commit message:
   
   ```bash
   git commit -m "Submitting OBJPROG Week 02 - Session 01 - Exercise 03"
   ```
   
4. Push your changes to GitHub:
   Upload your changes to your remote repository:
   
   ```bash
   git push origin main
   ```
