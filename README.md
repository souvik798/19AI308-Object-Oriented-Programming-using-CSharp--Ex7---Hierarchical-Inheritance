# AIM:
To write a C# program to implement heirarchical inheritance for the following problem statement: All the vehicles need Tyres on their wheels. So, the manufacturer designs their vehicle as they want and import Tyre from its base class and fit it into Wheels. They don’t need to design Tyre all the time. Once they designed the model and use it various times. Aim is to create a Scooter and Car vehicle where the Tyre is being inherited from vehicle class.

# ALGORITHM:
# Step 1:
Create a base class.

# Step 2:
Create two child class.

# Step 3:
Create a constructor in the base class and print a message.

# Step 4:
Inside the base class create a display function.

# Step 5:
Create constructor in child classes to print the message.

# Step 6:
Inside the child classes override the display functions.

# Step 7:
In the Main function, create an object for each child classes.

# PROGRAM:
```
using System;

namespace exp8
{
    public class tyre
    {
        public tyre() {
            Console.WriteLine("Tyre - Vehicle");
        }
        public virtual void display()
        {
            Console.Write("Tyre is attached to ");
        }
    }

    public class car : tyre
    {
        public car() {
            Console.WriteLine("Car Constructor");
        }
        public override void display()
        {
            base.display();
            Console.WriteLine("Car");
        }
    }

    public class scooter : tyre
    {
        public scooter() {
            Console.WriteLine("Scooter Constructor");
        }
        public override void display()
        {
            base.display();
            Console.WriteLine("Scooter");
        }
    }
    public class main
    {
        public static void Main(string[] args)
        {
            car newcar = new car();
            newcar.display();
            Console.WriteLine();
            scooter newscooter = new scooter();
            newscooter.display();
        }
    }
}
```
# OUTPUT:

![ex7](https://github.com/user-attachments/assets/2c3873ce-8d4d-48f5-8135-16ca13bbbff0)


# RESULT:
Thus, C# program to print some messages using hierarchical inheritance is implemented successfully.
