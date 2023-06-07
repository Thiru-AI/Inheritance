# Inheritance

## Aim:
To write a C# program to print some messages using hierarchical inheritance

## Algorithm:
### Step 1:
Create a base class Tyre.

### Step 2:
Create two child class.

### Step 3:
Create a constructor in the base class and print a message.

### Step 4:
create a function in child class to print a message.

### Step 5:
Run the program.

## Program:
~~~
using System;
namespace vehicles
{
    public class tyre
    {
        public tyre()
        {
            Console.WriteLine("constructor tyre");
        }
        public virtual void Display()
        {
            Console.WriteLine("tyre");
        }
    }
    public class scooter : tyre
    {
        public scooter()
        {
            Console.WriteLine("constructor scooter");
        }
        public override void Display()
        {
            base.Display();
            Console.WriteLine("scooter");
        }
    }
    public class car : tyre
    {
        public car()
        {
            Console.WriteLine("constructor car");
        }
        public override void Display()
        {
            base.Display();
            Console.WriteLine("car");
        }
    }
    public class GFG
    {
        public static void Main(string[] args)
        {
            scooter Scooter = new scooter();
            Scooter.Display();
            car Car = new car();
            Car.Display();
        }
    }
}
~~~

## Output:
![Screenshot (24)](https://github.com/Thiru-AI/Inheritance/assets/94980741/7e0b16c3-0a0a-4ffd-9631-7fc6f3067223)
## Result
Thus, C# program to print some messages using hierarchical inheritance.
