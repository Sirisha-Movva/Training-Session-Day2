# Training-Session-Day2
Lab 1 - 
  		Scanner scanner = new Scanner(System.in);
		System.out.print("Please enter your name : ");
		String name = scanner.next();
    
    Accept name and marks from user and show status as pass or fail (pass if marks>=35)
 ................................
 ..................................
 Lab 2- Eclipse
	Create a new class -> package - maths, class Name - Calc
	Write a method add in class Calc
			public int add(int no1, int no2) {
				return no1+no2;
			}
	Create a new class -> package -> defualt, class Name = Lab2
	Write a main method to invoke add from Calc class
		import java.util.Scanner;
		import maths.Calc;
		public class Lab2 {

			public static void main(String[] args) {
				Scanner scanner = new Scanner(System.in);
				System.out.print("Enter Number 1 : ");
				int no1 = scanner.nextInt();
				System.out.print("Enter Number 2 : ");
				int no2 = scanner.nextInt();

				Calc c1 = new Calc();
				int sum = c1.add(10, 20);
				System.out.println("Sum of 10 and 20 is " + sum);
				sum = c1.add(no1,  no2);
				System.out.println("Sum of " + no1 + " and " + no2 + " is " + sum);
			}
		}

	Write one more method - subtract -> accept two input number no1, no2 and return subtraction
	and invoke it from Lab2
  ...................................
  ................................................
  Lab 3 - 
	Create a new class -> Emp
		Create 3 fields (data members)
			private int empno;
			private String ename;
			private double salary;
		in class
			right click -> source -> generate constructor using field.
			right click -> source -> generate tostring method
	Create a new class -> Lab3 with main method
		Emp e1 = new Emp(1,"Sarita",1111.11);
		System.out.println(e1);
	Run 
	........................
  .................................
  Lab 5 - Modify Emp.java 
	in class
			right click -> source -> generate getters & settter for all three variables
	Modify Lab3.java to add 
		e1.setEname("Simantini");
		System.out.println(e1);
	run ...
Lab 4 - Write a method in Emp 
	-> void - no return, ()-> no input parameter
		public void incrSalary() {
		// this.salary = this.salary+ 100;
		this.salary += 100;
		}
	Modify Lab3.java to invoke incrSalary
		e1.incrSalary();
		System.out.println(e1);
	Add one more method incrSalary but with input parameter as percent
		public void incrSalary(int percent) {
			this.salary += this.salary*percent /100;
		}
	Modify Lab3.java to invoke incrSalary with parameter
		e1.incrSalary(10);
	Test ...
  ..................................
  ......................................
  Java Classes and Objects(https://www.w3schools.com/java/java_classes.asp)
	Attributes, methods, constructors,
  ........................................
  ..............................................
  Create Product.java
	-> int prodno, String prodname, String features, double cost
	-> generate -> constructor with params, getters/setters, toString
Write ProductCheck.java
	-> create a instance of Product(with constructor parameter
	-> invoke toString
	-> invoke setFeatures to modify features
	-> invoke toString
    
