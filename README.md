1) Write a program to accepts two numbers from stdin and find all the odd as well as even numbers present in between them.

import java.util.*;
public class Main {
	public static void main(String args[])
	{
		Scanner s=new Scanner(System.in);
		int a =s.nextInt(); //getting first number from user
		int b=s.nextInt(); //getting second number from user
		System.out.println("The even numbers are:");
for(int i=a;i<=b;i++)
{
	if(i%2==0)
		System.out.println(i);//display even numbers from input
}
System.out.println("The odd numbers are:");
for(int i=a;i<=b;i++)
{
	if(i%2!=0)
		System.out.println(i);//display odd numbers from input
}
	}

}

2)Joe is scared to go to school. When her dad asked the reason, joe said she is unable to complete the task given by her teacher. The task was to find the “first 10 multiples” of the number entered from stdin.


import java.util.Scanner;
public class Main {
public static void main(String args[]){
	Scanner s=new Scanner(System.in);
	int a=s.nextInt();//getting from user
	for(int i=1;i<=10;i++)//defining loop
	{
		System.out.println(a+"*"+i+"="+(a*i));//printing multiplication values(output)
	}
}
}


3)Write a program consisting method sum() and demonstrate the concept of method overloading using this method.

import java.util.Scanner;


public class Main {
public static void main(String args[])
{
	Scanner s=new Scanner(System.in);
System.out.println("1.Sum of two numbers \n2.Sum of three numbers");  
int i =s.nextInt();
if(i==1){
System.out.println("Enter two numbers");
int x=s.nextInt();
int y=s.nextInt();
sum(x,y);  //calling the method sum which accepts two integers
}
if(i==2){ System.out.println("Enter three numbers");
int b=s.nextInt();
int c=s.nextInt();
int d=s.nextInt();
sum(b,c,d);  //calling the method sum which accepts three integers
}
}
public static void sum(int a,int b)  //creating a method sum which accepts two integers
{
	System.out.println("Sum of two numbers are "+(a+b));
}
public static void sum(int a,int b,int c) //creating a method sum which accepts three integers
{
	System.out.println("Sum of three numbers are "+(a+b+c));
}
}
