# PrimeNumber
Checking input numbers for being Prime or not 
package Assignments2;

import java.util.Scanner;

public class PrimeNumber {
	public static void main(String[] args) {

		Scanner sc = new Scanner(System.in);
		System.out.println("Enter any number: ");
		int number = sc.nextInt();
		int i = 2;
		boolean primeNumber = false;
		while (i <= number / 2) {
			if (number % i == 0) {
				primeNumber = true;
				break;
			}
			++i;
		}
		if (!primeNumber) {
			System.out.println(number + " is a prime number");
		} else {
			System.out.println(number + " is not a prime number");
		}
		sc.close();

	}
}
