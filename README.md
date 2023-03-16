# Eligibility-for-Admission

## Aim:
To write C# program to find the eligibility for admission to an engineering course

## Algorithnm:
~~~
Start the program and declare the variables required.

Obtain the input from the user and read the values.

Calculate the total marks and check for the conditions.

Print the required output.

End the program.
~~~

## Program:

~~~
using System;
namespace exp1

{
     class Conversion
    {
        static void Main(String[] args)
        {
            int mat, phy, chem;
            string name;
            Console.Write("Enter the student name");
            name = Console.ReadLine();
            Console.Write("Enter the mark Scored in Maths:");
            mat = Convert.ToInt32(Console.ReadLine());
            Console.Write("Enter the marks scored in Physics:");
            phy = Convert.ToInt32(Console.ReadLine());
            Console.Write("Enter the marks scored in Chemistry:");
            chem = Convert.ToInt32(Console.ReadLine());
            int total1 = mat + phy + chem;
            int total2 = mat + phy;
            if (mat >= 65 && phy >= 55 && chem >= 50)
            {
                if (total1 > 180 || total2 > 140)
                {
                    Console.WriteLine(name + " is eligible for engineering admission.");
                }
                else
                {
                    Console.WriteLine(name + " is not eligible for engineering admission.");
                }

            }
            else
            {
                Console.WriteLine(name + "is not eligible for engineering admission.");
            }
        }
    }
 }
~~~

## Output:
![output](./C1.png)


## Result:
Thus,the program to find the eligibility for admission to an engineering course is executed successfully.
