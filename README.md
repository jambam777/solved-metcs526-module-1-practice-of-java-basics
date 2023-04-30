Download Link: https://assignmentchef.com/product/solved-metcs526-module-1-practice-of-java-basics
<br>
This assignment is practice of Java basics.

<strong>Problem 1</strong>. An incomplete Java program named <em>Hw1_P1_incomplete</em>.<em>java</em> is posted on the course website. You must complete the program by implementing the following requirements. Don’t forget to delete “<em>_incomplete</em>” from the file name.

This program has three methods. The first method receives an array of integers and calculates the average, the minimum, and the maximum of the integers and prints them on the screen.

The signature of this method is:

public static void stats(int[ ] numbers)




The second method creates and prints a subarray of a given array. The specification of the method is:

<ul>

 <li>Signature of method:</li>

</ul>

public static void subarray(int[ ] a, int from, int to)

<ul>

 <li>Input arguments:</li>

</ul>

<em>a</em>: An array of integers <em>from</em>: The index of an element in <em>a</em> which becomes the first element in the subarray <em>to</em>: The index of an element in <em>a</em> which becomes the last element in the subarray  Behavior:

<ul>

 <li>A new integer array is created, which is a subarray of <em>a</em>, and it includes elements <em>a</em>[<em>from</em>] to <em>a</em>[<em>to</em>], inclusively.</li>

 <li>Prints the subarray.</li>

 <li>There is no return value.</li>

</ul>

The third method is a main method. If you run this program with the following main method:

public static void main(String[] args) {

int[] a = {15, 25, 10, 65, 30, 55, 65};                System.out.print(“
Given array is: “);

for (int i=0; i&lt;a.length‐1; i++) {

System.out.print(a[i] + “, “);

}

System.out.print(a[a.length ‐ 1]);

System.out.println();




stats(a);

subarray(a, 1, 4);




Your output should be:




Given array is: 15, 25, 10, 65, 30, 55, 65

average = 37.86, min = 10, max = 65




The subarray, from index 1 to index 4, is: 25, 10, 65, 30

<strong>Problem 2 .</strong> For this problem, first you need to write a subclass of the <em>Employee</em> class. The definition of the <em>Employee</em> class is in the <em>Employee.java</em> file and it is briefly described below:

Class Employee

Instance variables  empId:

<ul>

 <li>Description: Employee id of an employee</li>

 <li>Type: integer  name:</li>

 <li>Description: Name of an employee</li>

 <li>Type: String</li>

</ul>

Instance methods:

<ul>

 <li>getEmpId</li>

 <li>No input argument</li>

 <li>Returns the employee id</li>

 <li>getName</li>

 <li>No input argument</li>

 <li>Returns the employee name</li>

 <li>setEmpId</li>

 <li>Input argument: empId of integer type</li>

 <li>Existing empId is replaced with the given empId</li>

 <li>No return value</li>

 <li>setName</li>

 <li>Input argument: name of String type</li>

 <li>Existing name (which may be null) is replaced with the given name  No return value</li>

</ul>




You need to implement the following class, which is a subclass of the <em>Employee</em> class. Define this class in a separate file named <em>SalariedEmployee.java</em>.

<h1>Class SalariedEmployee</h1>

<ul>

 <li>A subclass of the <em>Employee</em> class</li>

 <li>Instance variables</li>

 <li>salary: annual salary; double type</li>

 <li>Instance method</li>

 <li>monthlyPayment</li>

 <li>No input argument</li>

 <li>Returns monthly payment; double type</li>

 <li>Monthly payment is calculated as salary / 12</li>

 <li>employeeInfo</li>

 <li>No input argument</li>

 <li>Displays the empId, name, salary, and monthly payment</li>

 <li>No return value</li>

</ul>




In the subclass definition, you must implement all necessary <em>get methods</em> and <em>set methods</em>.

Then, write a program, named <em>Hw1_P2.java</em>, that reads employee information from a text file and stores <em>SalariedEmployee</em> objects in an array of size 10, named <em>employeeArray</em>, and displays employees satisfying a certain criterion. Follow the instruction below:

<ul>

 <li>Write a method, named <em>employeesAbove</em>, whose behavior is specified below:</li>

 <li>Signature of method:</li>

</ul>

public static void employeesAbove (SalariedEmployee[ ] empArray, double threshold)

<ul>

 <li>Input arguments: <em>empArray</em>: An array of <em>SalariedEmployee</em> objects <em>threshold</em>: A salary threshold</li>

 <li>Behavior: Selects from <em>empArray</em> only those employees who earn more than the given threshold amount, and displays their <em>empId</em>, <em>name</em>, <em>salary</em>, and monthly payment.</li>

 <li>There is no return value.</li>

 <li>In the main method, do the following:</li>

 <li>Read information of 10 salaried employees from an input file named <em>txt</em> and create 10 <em>SalariedEmployee</em> objects and store them in <em>employeeArray</em>. A sample input file is shown below:</li>

</ul>

1, John, 50000

2, Susan, 120000

3, Yapsiong, 80000

4, Gomez, 90000

5, Minsky, 60000

6, Yorst, 30000

7, Govindranad, 40000

8, Kelsey, 60000

9, Jake, 110000

10, Guanyu, 70000




<ul>

 <li>Invoke the <em>employeesAbove</em> method a few times with different threshold values and check that your output is correct. If, for example, you invoke the method with the threshold 70000, then the output should be:</li>

</ul>




Employees earning more than $70000:




Employee id = 2

Name = Susan

Salary = 120000.00

Monthly pay = 10000.00




Employee id = 3

Name = Yapsiong

Salary = 80000.00

Monthly pay =  6666.67




Employee id = 4

Name = Gomez

Salary = 90000.00

Monthly pay =  7500.00




Employee id = 9

Name = Jake

Salary = 110000.00

Monthly pay =  9166.67







<strong>Deliverable</strong>




No separate documentation is needed for the program files. However, you must include the following in your source code:

<ul>

 <li>Include the following comments above each method:</li>

 <li>Brief description of the method</li>

 <li>Input arguments</li>

 <li>Output arguments</li>

 <li>Include inline comments within your source code to increase readability of your code and to help readers better understand your code.</li>

</ul>


