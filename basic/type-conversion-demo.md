# Demo: Type Conversion

````csharp
namespace TypeConversion
{
    class Program
    {
        static void Main(string[] args)
        {
            byte b = 1;
            int i = b;

            int c = 1;
            byte j = c; // won't compile

            byte j2 = (byte)c; // works

            Console.WriteLine(i);

            // another example
            var number = "1234";
            int i = Convert.ToInt32(number);
            Console.WriteLine(i);
        }
    }
}
````

## Handling Exceptions with try...catch block

````csharp
namespace TypeConversion
{
    class Program
    {
        static void Main(string[] args)
        {
            try
            {
                var number = "1234";
                byte b = Convert.ToByte(number);
                Console.WriteLine(b);
            }
            catch (Exception)
            {
                Console.WriteLine("The number could not be converted to a byte!");
            }
        }
    }
}
````