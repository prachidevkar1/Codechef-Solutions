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


