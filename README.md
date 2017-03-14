# Simple-While-Loop-in-Java

001) The 'while' loop is the most basic iteration statement in Java.
002) Here's how a 'while' loop looks:

while(condition){
	//statements;
	}

003) Here, the 'condition' within the parenthesis is an expression that provides
     a Boolean output. The statments within the loop will only be executed if
     the condition is met. Otherwise, the loop is bypassed, and the program
     continues execution from after the loop.

004) Have a quick look at the following program that will help you understand
     how the 'while' loop works:

import java.util.Scanner;

public class simpleWhileLoop {

	public static void main(String[] args) {
		// TODO Auto-generated method stub

		Scanner scanner = new Scanner(System.in);
		System.out.println("Welcome to the Factorial Calculator.");
		System.out.println("Enter the number whose factorial you want to calculate: ");
		
		float number = scanner.nextFloat();
		float factorial = 1;
		float n = number;
		
		while(n > 0){
			factorial = n * factorial;
			--n;
		}
		
		System.out.println();
		System.out.println("The factorial of " + number + " is: " + factorial);
		
		
	}

}

005) The output proivided by this is:

Welcome to the Factorial Calculator.
Enter the number whose factorial you want to calculate: 
6

The factorial of 6.0 is: 720.0

006) Here, you see that while program execution enters the 'while' loop, it 
     checks for the condition 'n > 0'. If the Boolean equivalent is 'true',
     the statements within the parenthesis '{ }' are executed.
007) When the entire block of code has finished executing, the control goes back
     to 'while' and the condition is once again checked, and the whole process
     is repeated.
008) This goes on till the condition doesn't return a Boolean false equivalent,
     at which point the program exits the 'while' loop, and control shifts to
     the next statement after the loop.
