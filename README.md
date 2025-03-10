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


## Count of Digits et's assume the number of digits in N is x.Whenever we divide a number by 10 and store it in an integer, the right-most digit of that number gets removed.Since  digit gets removed each time we divide a number by 10 thus the total number digits we can remove from a number are the total number of digits in the number.
import java.util.Scanner;

class Codechef
{
	public static void main (String[] args) 
	{
		Scanner scanner = new Scanner(System.in);
        int num, count = 0;
        num = scanner.nextInt();

        while (num != 0) {
	
            num=(num/10);  //removing last digit
            count++;      //tracking the number of divisions
            
        }
        System.out.println(count);
	}
}


## Prime number 

public static void main (String[] args) 
	{
		Scanner scanner = new Scanner(System.in);

        int n = scanner.nextInt();
    
        boolean isPrime = true; // Assum n is prime.

        for(int i=2;i<n;i++)
        {
            if(n % i==0)
            {
                isPrime=false;
            }
           
        }
        if (isPrime) {
            System.out.println("Yes");
        } else {
            System.out.println("No");
        }
	}
}


## create a square pattern of integer N
import java.util.Scanner;

class Codechef
{
	public static void main (String[] args)
	{  
	    int i=1;
		Scanner scanner = new Scanner(System.in);
        int n = scanner.nextInt();
          for(i=1;i<=n;i++)
          {
              for(int j=1;j<=n;j++)
              {
                  System.out.print(" *");
                  
              }
              System.out.println();
          }
           
	}
}

## print Number patteren Right angled Triangle
import java.util.Scanner;

class Codechef
{
	public static void main (String[] args) 
	{
        Scanner scanner = new Scanner(System.in);
        int n = scanner.nextInt();
        
        for(int i=1;i<=n;i++)
        {
            for(int j=1;j<=i;j++)
            {
                System.out.print(j +" ");
            }
            System.out.println();
        }

	}
}

## Changing the elements of an Array
To change the value of a specific element, we can refer to the index number.
Task
Write a program which does the following:
The 3rd month in the given list is incorrect.
Update the 3rd month in the given array with the correct one - "Mar".
Once the 3rd array element is updated, output the 3rd array element to the console.
class Codechef
{
	public static void main (String[] args)
	{
		String[] months = {"Jan", "Feb", " Dec", "Apr"};
		months[2]="Mar";
		System.out.println(months[2]);
	}
}

## using for loop print last two days
class Codechef
{
	public static void main (String[] args)
	{
		String[] week = {"Monday", "Tuesday", "Wednesday", "Thursday"};
		 for(int i=2;i<week.length;i++)
		 {
		     System.out.println(week[i]);
		 }

	}
}

## Deletion from an array
Deleting elements from a 1D array involves removing an element from a specific position within the array and then shifting the remaining elements to fill the gap.
Determine the Position:
Shift Elements: Starting from the position of the element to be deleted, move each element one position to the left until you reach the end of the array. This fills the gap left by the deleted element.
Update Array Size

import java.util.Scanner;
class Codechef
{
	public static void main (String[] args) 
	{
		int[] array = new int[100]; 
			int[] arrays = new int[100]; // Initial array
            array[0] = 2;      
	    array[1] = 4;
	    array[2] = 6;
	    array[3] = 8;
	    array[4] = 10;
        int size = 5; // Current size of the array

        int positionToDelete = 2; // Index of the element to delete

        // Update the code to shift elements to fill the gap left by the deleted element
        
           for(int i=positionToDelete;i<size-1;i++)
           {
               array[i]=array[i + 1];
           }
           size--;
           
               
        // Print the updated array
        for (int i = 0; i < size; i++) {
            System.out.print(array[i] + " ");
        }
	}
}

## Insertion in an array
Inserting elements into a 1D array involves adding a new element at a specific position within the array.
import java.util.Scanner;

class Codechef
{
	public static void main (String[] args) 
	{
	    int []array = new int[100];
	    array[0] = 2;
	    array[1] = 4;
	    array[2] = 6;
	    array[3] = 8;
	    array[4] = 10;
        int size = 5; // Current size of the array

        int newPosition = 2; // Index where you want to insert the new element
        int newElement = 7; // Element to be inserted

        // Shift elements to make space for the new element
        for (int i = size - 1; i >= newPosition; i--) {
            array[i + 1] = array[i];
        }

        // Insert the new element at the specified position
        array[newPosition] = newElement;

         size++;// Update the size of the array

        // Print the updated array
        for (int i = 0; i < size; i++) {
            System.out.print(array[i] + " ");
        }

	}
}



## Merging Two Array
import java.util.Scanner;

class Codechef
{
	public static void main (String[] args) 
	{
		int firstArray[] = new int[100]; // First array
        firstArray[0] = 2;
        firstArray[1] = 4;
        firstArray[2] = 6;
        int size1 = 3;

        int secondArray[] = new int[100]; // Second array
        secondArray[0] = 8;
        secondArray[1] = 10;
        secondArray[2] = 12;
        secondArray[3] = 14;
        int size2 = 4;
        
        // Update the code below to solve the problem.
        int mergedSize= size1 + size2;
        int[] mergedArray= new int [mergedSize];
        for(int i= 0; i<size1;i++)
        {
            mergedArray[i]=firstArray[i];
            
        }
        for(int i= 0;i<size2;i++)
        { 
            mergedArray[size1 + i]=secondArray[i];
            
        
        }
        
        // Print the merged array
        for (int i = 0; i < mergedSize; i++) {
            System.out.print(mergedArray[i] + " ");
        }

	}
}

## Coding problem - 1 You are given the following as a user input: First line contains the integer N ,The second line contains N space separated integers. The third line contains an integer X.You need to insert X as the 1st and last element and output the list.Your list will now have N + 2 elements.

import java.util.Scanner;

class Codechef {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // Read the number of elements
        int N = sc.nextInt();
        int[] arr = new int[N];

        // Read N space-separated integers
        for (int i = 0; i < N; i++) {
            arr[i] = sc.nextInt();
        }

        // Read the integer X
        int x = sc.nextInt();

        // Create a new array with N+2 size
        int[] result = new int[N + 2];

        // Insert X at the beginning
        result[0] = x;

        // Copy original elements
        for (int i = 0; i < N; i++) {
            result[i + 1] = arr[i];
        }

        // Insert X at the end
        result[N + 1] = x;

        // Print the modified array
        for (int num : result) {
            System.out.print(num + " ");
        }

        sc.close();
    }
}
## You are given the following as a user input: First line contains the integer N and X The second line contains N space separated integers (List 1). The third line contains X space separated integers (List 2).
You need to merge the lists such that your output is a single list - List 1 + List 2 + List 1.
mport java.util.Scanner;

class Codechef {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // Read N and X
        int N = sc.nextInt();
        int X = sc.nextInt();

        // Read List 1
        int[] list1 = new int[N];
        for (int i = 0; i < N; i++) {
            list1[i] = sc.nextInt();
        }

        // Read List 2
        int[] list2 = new int[X];
        for (int i = 0; i < X; i++) {
            list2[i] = sc.nextInt();
        }

        // Print List 1
        for (int num : list1) {
            System.out.print(num + " ");
        }

        // Print List 2
        for (int num : list2) {
            System.out.print(num + " ");
        }

        // Print List 1 again
        for (int num : list1) {
            System.out.print(num + " ");
        }

        sc.close();
    }
}

## Let's solve a simple problem. Write a program which does the following:Accepts 5 inputs given on 5 separate lines. Each input is an integer N. For each test cases, prints out the integer N to console on a separate line (our Input mirror problem).
import java.util.Scanner;

class Codechef
{
	public static void main (String[] args)
	{
        Scanner read = new Scanner(System.in);
        
        String A = read.next();
        String B = read.next();
        String C = read.next();
        String D = read.next();
        String E = read.next();
        // You can use "\n" to add a new line instead of adding multiple print statements
        System.out.print(A + "\n" + B + "\n" + C + "\n" + D + "\n" + E );
	}
}
## Accepts the count of test cases - T - as an integer input given in the 1st line. This is followed by T lines - Each line contains an integer N. For each test cases, prints out the integer N to console on a separate line (our Input mirror problem).
// Update the '_' in the code below
import java.util.Scanner;

class Codechef
{
	public static void main (String[] args)
	{
        Scanner  read = new Scanner(System.in);
        // accept the count of test cases given in the 1st line
        int t = read.nextInt();
        
        // Run a loop to accept 't' inputs
        for(int i=0; i<t; i++)
        {
            // accept an integer N in each test case
            int n = read.nextInt();
            // output the number mirror for each test case
            // "println" prints output followed with a new line.
            System.out.println(n);
        }
	}
}



## The first line of input contains an integer t, the number of test cases. Each test case consists of: A line containing two integers a and b (separated by space).A line containing a string s.
import java.util.Scanner;

class Codechef
{
	public static void main (String[] args)
	{
        Scanner read = new Scanner(System.in);
        // accept the count of test cases given in the 1st line
        int t = read.nextInt();
        
        // Run a loop to accept 't' inputs
        for(int i=0; i<t; i++)
        {
            // accept 2 integers on the 1st line of each test case
            int a = read.nextInt();
            int b = read.nextInt();
            
            // accept 1 string on the 2nd line of each test case
            String s = read.next();
            
            // output the 2 integers and 1 string on a single line for each test case
            System.out.println(a + " " + b + " " + s);
        }
	}
}

## Write a program that utilizes a while loop to print the squares of numbers from 1 to 5.
class Codechef
{
	public static void main (String[] args) 
	{ int i= 1 ;
		while(i < 6)
		{
		    System.out.println(i*i);
		    i++;
		}
	}
}





## Write a program that uses a do-while loop to find the factorial of a given input number.


import java.util.Scanner;

class Codechef
{
	public static void main (String[] args)
{ 

     
     Scanner sc =new Scanner (System.in);
      int n = sc.nextInt();
      int factorial=1;
       int i=n;
      
      do{
          factorial= factorial*i;
          i--;
      }
      while(i>0);
        System.out.println(factorial);

	}
}


