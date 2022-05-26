# Operator-Overloading

## Aim:
 To write a C# program to find the volume of a box using operator overloading
 
 ##Algorithm:
 
 
 
 ##Program:
 ```c#
 using System;
class example
{
    public int length, breadth, hieght, volume;
    public static example operator +(example e1, example e2)
    {
        example e3 = new example();
        e3.length = e1.length + e2.length;
        e3.breadth = e1.breadth + e2.breadth;
        e3.hieght = e1.hieght + e2.hieght;
        e1.volume = e1.length * e1.hieght * e1.breadth;
        e2.volume = e2.length * e2.hieght * e2.breadth;
        e3.volume = e3.length * e3.hieght * e3.breadth;
        return e3;
    }
    public static void Main(string []args)
    {
        example e1 = new example();
        Console.WriteLine("Get 1st box length");
        e1.length = Convert.ToInt32(Console.ReadLine());
        Console.WriteLine("Get 1st box breadth");
        e1.breadth = Convert.ToInt32(Console.ReadLine());
        Console.WriteLine("Get 1st box hieght");
        e1.hieght = Convert.ToInt32(Console.ReadLine());
        example e2 = new example();
        Console.WriteLine("Get 2nd box length");
        e2.length = Convert.ToInt32(Console.ReadLine());
        Console.WriteLine("Get 2nd box breadth");
        e2.breadth = Convert.ToInt32(Console.ReadLine());
        Console.WriteLine("Get 2nd box hieght");
        e2.hieght = Convert.ToInt32(Console.ReadLine());
        example e3 = new example();
        e3 = e1 + e2;
        Console.WriteLine(e3.volume);
        Console.WriteLine("Volume of Box 1 is {0}\nVolume of Box 2 is {1}\nVolume of Box 3 is {2}", e1.volume, e2.volume, e3.volume);
    }
}


 ```
 ##Output:
 ![ss1](https://user-images.githubusercontent.com/75235150/170472060-a8270fe3-ec46-446c-990c-52981842cf3e.PNG)

 
 ##Result:
