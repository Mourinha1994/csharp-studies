# C# Basics - Progamming With Mosh

## Course content
- C# vs .NET
- CLR (Common Language Runtime)
- Architecture of .NET Applications
-  Our First C# Application

### C# vs .NET
- C# is a programming language.
- .NET is a framework for building applications on Windows
- .NET consists of two components: CLR and Class Library

### CLR (Common Language Runtime)
- Intermediate language between c#, VB, F# and machine code.
- Just in time compilation.
- With CLR we don't have to worry about compile code to different platforms because it will do all the work for us in runtime.

### Architecture of .NET Applications
- An application is built on one or many blocks of classes.
- A class is a container that contains data (attributes/properties) and behaviors (methods)
- For example, we can think of a car:

```csharp
public class Car
{
    public string Make { get; set; }
    public string Model { get; set; }
    public string Color { get; set; }

    public void Start()
    {
        Console.WriteLine("Engine started");
    }

    public void Move()
    {
        Console.WriteLine("Car is moving");
    }
}
```

- As far as our application grows, we need to organize all the pieces of code. This is the concept of namespace (a container for related classes).
- As far as our application grows more, we need to separate all the namespaces. This the concept of an Assembly. Assembly is a container for related namespaces. Physically an assembly is a file on the disk that can be either an executable (EXE) or a DLL (Dinamically Linked Library).
- When you compile your application, the compiler builds one more assemblies depending on how you partioned your code.

## Our First C# Application

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace BasicCSharp
{
    public class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello World!");
        }
    }
}
```

# Summary
## C# vs .NET
C# is a programming language, while .NET is a framework. It consists of a run-time environemnt and a class library the we use for building applications.

## CLR
When you compile an application, C# compiler compiles your code to IL (Intermediate Language) code. IL is platform agnostics, which makes it possible to take a C# program on a different hardware architecture and operating system and run it. For this to happen, we need CLR. When you run a C# application, CLR compiles the IL code into native machine code for the computer on which it is running. This process is called Just-in-time Compilation (JIT).

## Architecture of .NET Applications
In terms of architecture, an application written in C# consists of building blocks called classes. A class is a container for data and methods. Attributes represent the state of the application. Methods include code. They have logic. That's where we implement our algorithms and write code.
A namespace is a container for related classes. So as your application grows in size, you may want to group the related classes into various namespaces for better maintainability.
As the number of classes and namespaces even grow further, you may want to physically separate related namespaces into separate assemblies. An assembly is a file (DLL or EXE) that contains one or more namespaces and classes. An EXE file represents a program that can be executed. A DLL is a file that includes code that can be re-used across different programs.

[Next Article](primitive_types.md)