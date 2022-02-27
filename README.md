feb17 Assignment
1.)  Write a program to check for lower triangular matrix
import java.util.Scanner;
public class Lower_Matrix
{
public static void main(String args[])
    {
        int a[][] = new int[5][5];
        System.out.println("Enter the order of your Matrics ");
        System.out.println("Enter the rows:");
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        System.out.println("Enter the columns:");
        Scanner s = new Scanner(System.in);
        int m = s.nextInt();
        if(n == m)
         {        
             System.out.println("Enter your elements:");
              for(int i = 0; i < n; i++)
            {
                for(int j = 0; j < n; j++)
                {      
 
                     Scanner ss = new Scanner(System.in);
                     a[i][j] = ss.nextInt();
                     System.out.print(" ");
                 }
            }
              System.out.println("You have entered:");
              for(int i=0; i<n; i++)
               {
                for(int j=0;j<n;j++)
                {      
                     System.out.print(a[i][j] + " ");
                 }
                System.out.println("");
               }
              System.out.println("The Lower Triangular Matrix is:");
              for(int i=0;i<n;i++)
               {
                for(int j=0;j<n;j++)
                 {
 if(i>=j)
                   {
                     System.out.print(a[i][j] +" ");
                   }
                else
                {
                    System.out.print("0"+" ");
                } 
              }
            System.out.println("");
           }
        }
         else
        {
            System.out.println("you have entered improper order");
        }
   }
}
--------------------------------------------------------------------------------------------------------------
2  Find the sum of diagonal elements of a matrix
import java.util.*;
 
public class arr16
{  
 public static void main(String args[])
 {
 Scanner sc = new Scanner(System.in);
 
         int i,j,row,col,sum=0;
 System.out.println("Enter the number of rows:");
 row = sc.nextInt();
 System.out.println("Enter the number of columns:");
 col = sc.nextInt();
 
 int[][] mat = new int[row][col];
 
     System.out.println("Enter the elements of the matrix") ;
     for(i=0;i<row;i++)
     { 
      for(j=0;j<col;j++)
      { 
          mat[i][j] = sc.nextInt();
     }
 }
 
     System.out.println("The elements of the matrix") ;
     for(i=0;i<row;i++)
     { 
      for(j=0;j<col;j++)
      { 
        System.out.print(mat[i][j]+"\t");
     }
       System.out.println("");
 }
 
     for(i=0;i<row;i++)
     { 
      for(j=0;j<col;j++)
 { 
 if(i==j) 
 {
 sum = sum + mat[i][j];
 }
     }
 }
 
     System.out.printf("SUM of DIAGONAL elements of the matrix = "+sum) ;
 } 
}
----------------------------------------------------------------------------------------------------------------
3 Check whether the matrix is sparse."

import java.util.Scanner;
public class Sparse
{
    public static void main(String args[])
    {
 	int i, j, zero = 0, count = 0; 
 	int array[][] = new int[10][10];
 	System.out.println("Enter total rows and columns: ");
 	Scanner s = new Scanner(System.in);
 	int row = s.nextInt();
 	int column = s.nextInt();
 	System.out.println("Enter matrix:");
        for(i = 0; i < row; i++)
        {
            for(j = 0; j < column; j++) 
    	    {
                 array[i][j] = s.nextInt();
                 System.out.print(" ");
    	     }
        }
        for(i = 0; i < row; i++)
        {
 	    for(j = 0; j < column; j++) 
  	    {
                if(array[i][j] == 0)
    		{
        	    zero++; 
    		}
    	   	else
            	{
      	            count++;
    	    	}
   	   }
       }
       if(zero>count)
       {
           System.out.println("the matrix is sparse matrix");
       }
 else
       {
           System.out.println("the matrix is not a sparse matrix");
       }
    }
}
------------------------------------------------------------------------------------------------------------------
FEB18 Assignments
1 .Create a class named 'Student' with String variable 'name' and integer variable 'roll_no'.
 Assign the value of roll_no as '2' and that of name as "John" by creating an object of the class Student.

public class Student {
private  String name;
	private int rollno;
	public Student() {
		
	}
	public Student(String name,int age) {
		name=name1;
		rollno=rollno1;
	}
	
	public String getName() {
		return name;
	}
	public int getRollno() {
		return rollno;
		
	}
	public String displayStudentDetails() {
		return getName()+" "+getRollno();
		
	}

}

public class main {
	public static void main(String[]args) {
		Student obj1=new Student();
	String displayStudentDetails = obj1.displayStudentDetails();
	System.out.println("student details:"+ StudentDetails);
	Student obj2 =new Student(name:"keerthi",rollno:78);
	String displayStudentDetails1 = obj1.displayStudentDetails();
	System.out.println("student details:"+ StudentDetails1);
	
		
	}

}
---------------------------------------------------------------------------
2 Assign and print the roll number, phone number and address of two students having names "Sam" and 
"John" respectively by creating two objects of class 'Student

public class studentDetails {
	public String name;
	public int rollNumber;
	public long mobileNumber;
	public static String getName(String name) {
		return name;
		
	}
	public static int getRollNum(int roll) {
		return roll;
	}
	public static long getMobileNum(long num) {
		return num;
	}

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		studentDetails obj=new studentDetails();
		String name=obj.getName("sam");
		int num=obj.getRollNum(01);
		long mobile=obj.getMobileNum(6337934461l);
		System.out.println("Details of sam : " +name +" "+num+" "+mobile);
		String name1=obj.getName("john");
		int num1=obj.getRollNum(02);
		long mobile1=obj.getMobileNum(9629730877l);
		System.out.println("Details of john : " +name1 +" "+num1+" "+mobile1);
}

}
---------------------------------------------------------------------------
3 Create a class 'Employee' with String variable 'name' and integer variable 'employee id'. Create 4 Employee objects 
and store in array and display.
public class employee {
	public String name;
	public int id;
	public static String getName(String name) {
		return name;
		
	}
	public static int getRollNum(int roll) {
		return roll;
	}
	public static long getMobileNum(long num) {
		return num;
	}

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		studentDetails obj=new studentDetails();
		String name=obj.getName("sam");
		int num=obj.getRollNum(01);
		long mobile=obj.getMobileNum(6337934461l);
		System.out.println("Details of sam : " +name +" "+num+" "+mobile);
		String name1=obj.getName("john");
		int num1=obj.getRollNum(02);
		long mobile1=obj.getMobileNum(9629730877l);
		System.out.println("Details of john : " +name1 +" "+num1+" "+mobile1);
}

}
---------------------------------------------------------------------------
feb 21 homework
1. Modify the class to add a isTails method that returns true when the value is not heads.

public class Coin
{

   
   private static int tail = 1;

   
   private int value = 0;

 
   public void flip()
   {
      if (Math.random() < 0.5)
      {
          value = 0;
      }
      else
      {
         value = 1;
      }
   }

   
   public boolean istail()
   {
      return value == tail;
   }
   public String toString()
   {
      if (value == tail) return "tail";
      else return "Head";
   }
public static void main(String[] args)
   {

      Coin myCoin = new Coin();
      for (int i = 0; i < 10; i++)
      {
         myCoin.flip();
         System.out.println(myCoin);
         System.out.println(myCoin.istail());
      }
   }
}
-----------------------------------------------------------------------------------------------------
2  Modify the code below to add more constructors. Also modify the main method to test the new constructors.

public class Person
{
   // fields
   private String name;
   private String email;
   private String phoneNumber;

   // constructor
   public Person(String theName)
   {
      this.name = theName;
      this.email = theEmail;
      this.phoneNumber = thePhoneNumber;
   }

   // methods - getters
   public String getName() { return this.name;}
   public String getEmail() { return this.email;}
   public String getPhoneNumber() { return this.phoneNumber;}

   // methods - setters
   public void setName(String theName) { this.name = theName;}
   public void setEmail(String theEmail) {this.email = theEmail;}
   public void setPhoneNumber(String thePhoneNumber) { this.phoneNumber = thePhoneNumber;}
   public String toString()
   {
      return this.name + " " + this.email + " " + this.phoneNumber;
   }
--------------------------------------------------------------------------------------------------------------
3 package pack1;
 
 public class A
{
    public A()
    {
        
    }
}
 
package pack2;
 
import pack1.*;
 
class B
{
    A a = new A();   	
}
-----------------------------------------------------------------------------------------------------------------

feb22 
1. Edit this code so the class Beagle is a subclass of the Dog class. When you run the code it should print “woof!” and then “arf arf”

public class Dog
{
    public void speak()
    {
        System.out.println("woof!");
    }

    public static void main(String[] args)
    {
        Dog d = new Dog();
        d.speak();
       
    }
}

class Beagle
{
    public void speak()
    {
        System.out.println("arf arf");
    }
}
-----------------------------------------------------------------------------------------------------------------
2 public class Dog
{
    private String name;

    public Dog(String name)
    {
        this.name = name;
    }

    public boolean equals(Object other)
    {
        
    }

    public static void main(String[] args)
    {
        Dog d1 = new Dog("Rufus");
        Dog d2 = new Dog("Sally");
        Dog d3 = new Dog("Rufus");
        Dog d4 = d3;
        System.out.println(d1.equals(d2));
        System.out.println(d2.equals(d3));
        System.out.println(d1.equals(d3));
        System.out.println(d3.equals(d4));
    }
}
--------------------------------------------------------------------------------------------------------------------
feb23
create class animal with various.......

public class Animal {
	String talk;
	String eat;
	String drink;
	public static void getTalk() {
		System.out.println("Animal can talk with there language");
	}
	public static void getEat() {
		System.out.println("different animals can eat different things");
	}
	public static void getDrunk() {
		System.out.println("Animals can drink water");
	}

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Animal a=new Animal();
		a.getTalk();
		a.getEat();
		a.getDrunk();

	}

}
------------------------------------------------------------------------------------------------------------
create multiple objects like dog ,cat,cow ,elephant............
public class Dog {
	public void Speak() {
        System.out.println("woof!");

	}
	class Beagle extends Dog{
		public  void Speak() {
	        System.out.println("arf arf");

		}
	}

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Dog d=new Dog();
		d.Speak();
		Dog b=d.new Beagle();
		b.Speak();

	}
-------------------------------------------------------------------------------------------

feb 24 assignments 
1. Override the taste method from the Candy class in the Chocolate class to return “tastes chocolately”. It should print “tastes sweet!” and then “tastes chocolately”.

public class candy {
	 public String taste()
	    {
	        return "tastes sweet!";
	    }
	 class Chocolate extends candy
		{
		 public String taste()
		    {
		        return  "tastes chocolately";
		    }
		}

	    public static void main(String[] args)
	    {
	        candy c1 = new candy();
	        System.out.println(c1.taste());
	        candy c2 = c1.new Chocolate();
	        System.out.println(c2.taste());
	    }
	}
---------------------------------------------------------------------------------------------------------------------
2. When a subclass inherits from a superclass, it also inherits its methods; however, it can also override the superclass methods (as well as declare and implement new ones). Consider the following Sports class:
-----------------------------------------------
Write a method that overloads the talk method by taking in a name and printing “Hello” with that name.

public class Test1
{
    public static void talk()
    {
          System.out.println("hello there!");
    }

    public static // FINISH THE METHOD HERE //

    public static void main(String[] args)
    {
          talk("Matthew");
    }
}

--------------------------------------------------------------------------------------------------------------

feb 25assignment 
 1  class Automobile {
    private String drive() {
        return "Driving vehicle";
    }
}

class Car extends Automobile {
    protected String drive() {
        return "Driving car";
    }
}

public class ElectricCar extends Car {

    @Override
    public final String drive() {
        return "Driving electric car";
    }

    public static void main(String[] wheels) {
        final Car car = new ElectricCar();
        System.out.print(car.drive());
    }
}

B. Driving electric car
---------------------------------------------------------------------------------------------------------------------------
2Q - Look at the following code and choose the right option for the word :
// Shape.java
public class Shape {
    protected void display() {
        System.out.println("Display-base");
    }
}
// Circle.java
public class Circle extends Shape { <
    < access - modifier > void display() {
        System.out.println("Display-derived");
    }
}
a. Only protected can be used
-----------------------------------------------------------------------------------------------------------------------
Q3 - What will be the output of the following program?
class Base {
    public Base() {
        System.out.println("Base");
    }
}

class Derived extends Base {
    public Derived() {
        System.out.println("Derived");
    }
}

class DeriDerived extends Derived {
    public DeriDerived() {
        System.out.println("DeriDerived");
    }
}

public class Test {
    public static void main(String[] args) {
        Derived b = new DeriDerived();
    }
}
a)
Base
Derived
DeriDerived
--------------------------------------------------------------------------------------------------------------------------
Q4 - Consider the following program:
class Base {
    public Base() {
        System.out.print("Base ");
    }

    public Base(String s) {
        System.out.print("Base: " + s);
    }
}

class Derived extends Base {
    public Derived(String s) {
        super(); // Stmt-1
        super(s); // Stmt-2
        System.out.print("Derived ");
    }
}

class Test {
    public static void main(String[] args) {
        Base base = new Derived("Hello ");
    }
}
Select three correct options from the following list:

c) Removing Stmt-2 will make the program compilable and it will print the following: Base Derivered
---------------------------------------------------------------------------------------------------
Q5 - What is the output of the following application?
abstract class Car {
    static {
        System.out.print("1");
    }

    public Car(String name) {
        super();
        System.out.print("2");
    }

    {
        System.out.print("3");
    }
}

public class BlueCar extends Car {
    {
        System.out.print("4");
    }

    public BlueCar() {
        super("blue");
        System.out.print("5");
    }

    public static void main(String[] gears) {
        new BlueCar();
    }
}
C. 13245

-----------------------------------------------------------------------------------------------------------------
Q6 - What is the output of the following application?
class Math {
    public final double secret = 2;
}

class ComplexMath extends Math {
    public final double secret = 4;
}

public class InfiniteMath extends ComplexMath {
    public final double secret = 8;

    public static void main(String[] numbers) {
        Math math = new InfiniteMath();
        System.out.print(math.secret);
    }
}
A. 2
---------------------------------------------------------------------------------------------------
Q7 - Consider the following program and predict the output:
public class Test {
    public void print(Integer i) {
        System.out.println("Integer");
    }

    public void print(int i) {
        System.out.println("int");
    }

    public void print(long i) {
        System.out.println("long");
    }

    public static void main(String args[]) {
        Test test = new Test();
        test.print(10);
    }
}

d) int
--------------------------------------------------------------------------------------------------------------------------------------------


 










