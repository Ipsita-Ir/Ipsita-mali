# Ipsita-mali
Java

public class Calculator {

    // Addition
  public double add(double a, double b) {
        return a + b;
    }

    // Subtraction
  public double subtract(double a, double b) {
        return a - b;
    }

    // Multiplication
   public double multiply(double a, double b) {
        return a * b;
    }

    // Division with error handling for division by zero
   public double divide(double a, double b) {
        if (b == 0) {
            System.out.println("Error: Division by zero is not allowed.");
            return Double.NaN; // or throw an exception
        }
        return a / b;
    }

    // Main method to test the Calculator
   public static void main(String[] args) {
        Calculator calc = new Calculator();

System.out.println("Addition: " + calc.add(10, 5));         // Output: 15.0
        System.out.println("Subtraction: " + calc.subtract(10, 5)); // Output: 5.0
        System.out.println("Multiplication: " + calc.multiply(10, 5)); // Output: 50.0
        System.out.println("Division: " + calc.divide(10, 5));      // Output: 2.0
        System.out.println("Division by zero: " + calc.divide(10, 0)); // Output: NaN with error message
    }
}

Notes:

This version uses double to handle both integers and decimals.

Division by zero is handled by printing an error message and returning Double.NaN (Not a Number). You can change this to throw an exception if needed.


Would you like this adapted for integers only or with exception handling instead?

