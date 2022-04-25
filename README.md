# Combination
Java101_19 this program calculates combination of two given numbers

https://www.patika.dev/tr

// Combination formula ; C(n,r) = n! / (r! * (n-r)!)

import java.util.Scanner;
public class Main
{
    static int factorial(int num) {
        int i, factorialSum ;
        
        factorialSum = 1;

        for (i=1 ; i <= num; i++) {
            factorialSum *= i;
        }
        return factorialSum;
    }
	public static void main(String[] args) {
	    
	    int n, r, total ;
	    total=1;
	    Scanner input=new Scanner(System.in) ;
	    System.out.print("Enter n number : ");
	    n=input.nextInt();
	    
	    System.out.print("Enter r number : ");
	    r=input.nextInt();
	  
        total=factorial(n)/(factorial(r)*factorial(n-r));
        System.out.print("Combination of("+n+","+r+") is : "+total);	    
	  
	}
}
