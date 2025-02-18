# Codechef-Solutions

# 🚀 CodeChef Problem Solutions

This repository contains my solutions to various **CodeChef** problems. Each solution is implemented in **Java/C++/Python**, and the problem statements are documented here.

---

## 📌 Problem: Odd Numbers from 10 to 20
### 📝 Problem Statement
Print all **odd numbers** between `10` and `20`.

### ✅ Input
- No input required.

### 🎯 Output

Write a program to print odd numbers between 10 to 20
import java.util.Scanner;

class Codechef
{
	public static void main (String[] args) 
	{
	   // Update the code below this line.
	    int i = 11;
	    while(i < 20){
	        
	        if(i% 2!=0)
	        {
	            System.out.println(i);
	        }
	        i++;
	        
	    }
	}
}





## 📌 Print Numbers 5 - 20
import java.util.Scanner;

class Codechef
{
	public static void main (String[] args) 
	{
	    int i = 5; // Initialization
		while (i<=20) { // Condition
            System.out.println(i);
            i++; // Update statement
        }

	}
}

## Write a program which does the following:

Declare a variable num and store a user defined input from the console in it.
Declare a variable a and initialize it to 0
Use the syntax above to create a loop, output the following to the console:
Print a in separate lines as long as it is less than num.
Increment a by  1 in each iteration.
import java.util.Scanner;
class CodeChef{
    public static void main(String args[])
    {
        Scanner sc=new Scanner(System.in);
        int num =sc.nextInt();
        int a = 0;
        while((a<num))
        { 
            System.out.println(a);
            a++;
            
        }
    
    }
}


## Print powers of 2 up to 7 th 
import java.util.Scanner;

class Codechef
{
	public static void main (String[] args) 
	{
	 int num =1;
	 int a=2;
	 while((num<=7))
	 {
	     int result= (int) Math.pow(a,num);
	     System.out.println(result);
	     num++;
	 }
	
       
	}
}


## Sum of N IntegersChef was given an integer input N.He wants to write a code using while loops to output the sum of all integers from 1 to N
import java.util.Scanner;

class Codechef
{
	public static void main (String[] args) 
	{
		Scanner scanner = new Scanner(System.in);
        
        int i=1;
        int N, sum = 0;
        N = scanner.nextInt();

        while (i <= N) {
            sum += i;
            i++;
        }
        System.out.println(sum);
	}
}


## N The factorial of a number N is the product of each number from 1 to N!(N factorial)=1*2..N
import java.util.Scanner;

class Codechef
{
	public static void main (String[] args) 
	{
        Scanner scanner = new Scanner(System.in);
        int N, factorial = 1;   
        N = scanner.nextInt();  

        int i = 1;
        while (i <= N) {        
            factorial = factorial * i;     
            i++;
        }
        System.out.println(factorial);
	}
}


