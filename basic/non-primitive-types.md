# Non-Primitive Types

## Classes:
A class combines different variables (fields) and functions (methods). 
````csharp
class Person
{
    public string Name { get; set; }
    public byte Age { get; set; }
    public float Height { get; set; }
    public byte wieght { get; set; }

    public void Walk()
    {
        // TODO...
    }

    public void Talk()
    {
        // TODO...
    }

    public void Eat()
    {
        // TODO...
    }

    public void Sleep()
    {
        // TODO...
    }

}
````

 ## Objects:
 An object is an instance of class.

````csharp
class Program
{
    static void Main(string[] args)
    {
        Person p = new Person();

        p.Name = "Erick";
        p.Age = 26;
        p.Height = 1.65f;
        p.Weight = 50;

        p.Walk();
        p.Eat();
        p.Sleep();
    }
}
````

## Structs:
As well as Classes, structs combine related fields and methods. They aren't so used as classes.

````csharp
public struct RgbColors
{
    public int Red;
    public int Green;
    public int Blue;
}
````

## Arrays:
- What is an Array
- Declaring an Array
- Initializing Arrays
- Access Array Elements.