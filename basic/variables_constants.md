# Declaring Variables - DEMO


## Declaring Variables using primitive types:

````csharp
using System;

namespace Variables
{
    class Program
    {
        static void Main(string[] args)
        {
            int number = 2;
            int count = 10;
            float totalPrice = 10.29f;
            char character = 'A';
            string name = "Erick";
            bool isWorking = true;

            Console.WriteLine(number);
            Console.WriteLine(count);
            Console.WriteLine(totalPrice);
            Console.WriteLine(character);
            Console.WriteLine(name);
            Console.WriteLine(isWorking);
        }
    }
}
````

## Declaring variables using the "var" keyword:

````csharp
using System;

namespace Variables
{
    class Program
    {
        static void Main(string[] args)
        {
            // automatically inferes the variable type
            var number = 2;
            var count = 10;
            var totalPrice = 10.29f;
            var character = 'A';
            var name = "Erick";
            var isWorking = true;

            Console.WriteLine(number);
            Console.WriteLine(count);
            Console.WriteLine(totalPrice);
            Console.WriteLine(character);
            Console.WriteLine(name);
            Console.WriteLine(isWorking);
        }
    }
}
````

## Format Strings:

````csharp
using System;

namespace Variables
{
    class Program
    {
        static void Main(string[] args)
        {
            // zero represents the first argument and one represents the second argument
            Console.WriteLine("{0} - {1}", byte.MinValue, byte.MaxValue);
        }
    }
}
````

## Constants

````csharp
using System;

namespace Variables
{
    class Program
    {
        static void Main(string[] args)
        {
            // because we declare Pi as a constant, we cannot change the value.
            const float Pi = 3.14f;
            Pi = 1; // wrong
        }
    }
}
````
