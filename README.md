# AWP-prac-1a-
Practical No.: 1
AIM:- Working with basic C# and ASP .NET
A)Create an application that obtains four int values from the 
user and displays the product.
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
namespace ConsoleApplication1
{
 class Program
 {
 static void Main(string[] args)
 {
 int num1, num2, num3, num4, prod;
 Console.Write("Enter number 1: ");
 num1 = Int32.Parse(Console.ReadLine());
 Console.Write("Enter number 2: ");
 num2 = Convert.ToInt32(Console.ReadLine());
 Console.Write("Enter number 3: ");
 num3 = Convert.ToInt32(Console.ReadLine());
 Console.Write("Enter number 4: ");
 num4 = Convert.ToInt32(Console.ReadLine());
 prod = num1 * num2 * num3 * num4;
 Console.WriteLine(num1 + "*" + num2 + "*" + num3 + "*" + num4 + 
"=" + prod);
 Console.ReadKey();
 }
 }
(B) demonstrate string operation 
using System;
namespace cmdLineArgs
{
class Program
{
static void Main(string[] args)
{
string str = args[0];
int n = Convert.ToInt32(args[1]);
Console.WriteLine("String:" + str);
Console.WriteLine("Number:" + n);
}
}
}
OUTPUT:
String : Roman
Number : 10
(C) Application recieved 

using System;
namespace ArrayOfStructs
{
class Program
{
struct Student
{
public string studid, name, cname;
public int day, month, year;
}
static void Main(string[] args)
{
Student[] s = new Student[5];
int i;
for (i = 0; i < 5; i++)
{
Console.Write("Enter Student Id:");
s[i].studid = Console.ReadLine();
Console.Write("Enter Student name : ");
s[i].name = Console.ReadLine();
Console.Write("Enter Course name : ");
s[i].cname = Console.ReadLine();
Console.Write("Enter date of birth\n Enter day(1-31):");
s[i].day = Convert.ToInt32(Console.ReadLine());
Console.Write("Enter month(1-12):");
s[i].month = Convert.ToInt32(Console.ReadLine());
Console.Write("Enter year:");
s[i].year = Convert.ToInt32(Console.ReadLine());
}
Console.WriteLine("\n\nStudent's List\n");
for (i = 0; i < 5; i++)
{
Console.WriteLine("\nStudent ID : " + s[i].studid);
Console.WriteLine("\nStudent name : " + s[i].name);
Console.WriteLine("\nCourse name : " + s[i].cname);
Console.WriteLine("\nDate of birth(dd-mm-yy) : " + s[i].day + "-" + 
s[i].month +
"-" + s[i].year);
} } } }
1)C) OUTPUT:
Enter Student Id:0001
Enter Student name : Prachit
Enter Course name : MSCit
Enter date of birth
Enter day(1-31):29
Enter month(1-12):9
Enter year:1995
Enter Student Id:0002
Enter Student name : Aniket
Enter Course name : Bscit
Enter date of birth
Enter day(1-31):4
Enter month(1-12):3
Enter year:1996
Enter Student Id:0003
Enter Student name : Prathamesh
Enter Course name : BMS
Enter date of birth
Enter day(1-31):9
Enter month(1-12):8
Enter year:2000
Enter Student Id:0004
Enter Student name : Sumit
Enter Course name :MScet
Enter date of birth
Enter day(1-31):25
Enter month(1-12):5
Enter year:1994
Enter Student Id : 0005
Enter Student name : Zaid
Enter Course name : BCOM
Enter date of birth
Enter day(1-31):6
Enter month(1-12):7
Enter year:1993
Student's List
Student ID : 0001
Student name : Prachit
Course name : MSCit
Date of birth(dd-mm-yy) : 29-9-1995
Student ID : 0002
Student name : Aniket
Course name : Bscit
Date of birth(dd-mm-yy) : 4-3-1996
Student ID : 0003
Student name : Prathamesh
Course name : BMS
Date of birth(dd-mm-yy) : 9-8-2000
Student ID : 0004
Student name : Sumit
Course name : MScet
Date of birth(dd-mm-yy) : 25-5-1994
Student ID : 0005
Student name : Zaid
Course name : BCOM
Date of birth(dd-mm-yy) : 6-7-1993
