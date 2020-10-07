# Overflowing and Scope:

## Overflowing:

Happen when you try to exceed the boundaries of types's range.

````csharp
byte number = 255;
number = number + 1; // 0
````
To avoid overflowing, we must use the **checked** keyword:

````csharp
checked
{
    byte number = 255;
    number = number + 1; // program will throw an exception
}
````

## Scope:
Is where a variable / constant has meaning and is accessible.

````csharp
{
    byte a = 1;

    {
        byte b = 2;

        {
            byte c = 3;
        }
    }
}
````
- Variable **a** is accessible in any of child blocks of code;
- Variable **b** is accessible in just the inner block;
- Variable **c** is accessible in just its own scope;
