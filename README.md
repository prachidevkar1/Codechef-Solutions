# Codechef-Solutions

# 🚀 CodeChef Problem Solutions

This repository contains my solutions to various **CodeChef** problems. Each solution is implemented in **Java**, and the problem statements are documented here.

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

OR USING FOR LOOP
class OddNumber {
    public static void main(String[] args) {
        for (int i = 10; i <= 20; i++) {
            if (i % 2 != 0) {
                System.out.println("Odd Number: " + i);
            } else {
                System.out.println("Even Number: " + i);
            }
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

## array of string 
class Codechef {
    public static void main (String[] args) {
        String[] array = {"1", "ab", "3", "name"}; // Array with string values
        
        // Using a for loop
        for (int i = 0; i < array.length; i++) {
            System.out.println(array[i]); // Print each element on a new line
        }
    }
}

## Let us define a variable N that accepts integer inputs. Output the same variable N

import java.util.Scanner;

class Codechef
{
	public static void main (String[] args)
	{
        Scanner objName = new Scanner(System.in);
        int N = objName.nextInt();
		System.out.println(N);
	}
}



## Chef wants to become fit for which he decided to walk to the office and return home by walking. It is known that Chef's office is X km away from his home. If his office is open on 5 days in a week, find the number of kilometers Chef travels through office trips in a week. Input Format First line will contain T, number of test cases. Then the test cases follow. Each test case contains of a single line consisting of single integer  X
mport java.util.*;

class CodeChef {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int t = sc.nextInt(); // Number of test cases

        for (int i = 0; i < t; i++) { // Loop for each test case
            int x = sc.nextInt(); // Read distance X
            int totalDistance = 2 * x * 5; // Calculate total distance
            System.out.println(totalDistance); // Print the result
        }
        
        sc.close(); // Close the scanner
    }
}
## Second Max of Three Numbers Problem Statement Write a program that accepts sets of three numbers, and prints the second-maximum number among the three. Input First line contains the number of triples, N The next N lines which follow each have three space separated integers.
import java.util.*;
import java.lang.*;
import java.io.*;

import java.util.*;

class Codechef {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
        int N = sc.nextInt(); // Number of test cases

        for (int i = 0; i < N; i++) {
            int a = sc.nextInt();
            int b = sc.nextInt();
            int c = sc.nextInt();

            // Find the second maximum using sorting
            int[] arr = {a, b, c};
            Arrays.sort(arr);

            System.out.println(arr[1]); // Print the second maximum
        }

        sc.close();
    }
}
## Chef and Chocolates Chef has X 5 rupee coins and Y 10 rupee coins. Chef goes to a shop to buy chocolates for Chefina where each chocolate costs  Z rupees. Find the maximum number of chocolates that Chef can buy for Chefina.Input FormatThe first line contains a single integer T — the number of test cases. Then the test cases follow.The first and only line of each test case contains three integers X Y and Z — the number of 5 rupee coins, the number of 10 rupee coins and the cost of each chocolate.
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int t = scanner.nextInt();

        while (t-- > 0) {
            int x = scanner.nextInt(); // number of 5 rupee coins
            int y = scanner.nextInt(); // number of 10 rupee coins
            int z = scanner.nextInt(); // cost of one chocolate

            int amount = (5 * x) + (10 * y); // total money Chef has
            int chocolates = amount / z; // maximum chocolates that can be bought

            System.out.println(chocolates);
        }
    }
}
## Find Remainder Write a program to find the remainder when an integer A is divided by an integer B.Input The first line contains an integer T, the total number of test cases. Then T lines follow, each line contains two Integers A and B.
import java.util.*;
import java.lang.*;
import java.io.*;

class Codechef
{
    public static void main (String[] args) throws java.lang.Exception
    {
        Scanner sc = new Scanner(System.in);
        int t = sc.nextInt(); // number of test cases
        
        for (int i = 0; i < t; i++) // run t times
        {
            int A = sc.nextInt();
            int b = sc.nextInt();
            int remainder = A % b;
            System.out.println(remainder);
        }
    }
}

## Candy Store Chef has started working at the candy store. The store has  100 chocolates in total. Chef’s daily goal is to sell X chocolates. For each chocolate sold, he will get 1 rupee. However, if Chef exceeds his daily goal, he gets 2 rupees per chocolate for each extra chocolate.If Chef sells Y chocolates in a day, find the total amount he made. Input Format The first line of input will contain a single integer T, denoting the number of test cases. Each test case consists of two space-separated integers X and Y — the daily goal of Chef, and the number of chocolates he actually sells.
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int T = sc.nextInt(); // Number of test cases

        for (int i = 0; i < T; i++) {
            int X = sc.nextInt(); // Daily goal
            int Y = sc.nextInt(); // Chocolates sold

            int total;
            if (Y <= X) {
                total = Y;
            } else {
                total = X + (Y - X) * 2;
            }

            System.out.println(total);
        }

        sc.close();
    }
}
## Scalene TriangleGiven A,B, and C as the sides of a triangle, find whether the triangle is scalene. Note: A triangle is said to be scalene if all three sides of the triangle are distinct. It is guaranteed that the sides represent a valid triangle. Input Format The first line of input will contain a single integer T denoting the number of test cases. Each test case consists of three space-separated integers A,B and C — the length of the three sides of the triangle.
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int t = scanner.nextInt();

        while (t-- > 0) {
            int a = scanner.nextInt();
            int b = scanner.nextInt();
            int c = scanner.nextInt();

            if (a != b && b != c && a != c) {
                System.out.println("YES");
            } else {
                System.out.println("NO");
            }
        }
    }
}
