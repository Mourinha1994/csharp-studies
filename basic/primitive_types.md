# Primitive Types and Expressions

## Variables and Constants
- **Variables:** a name given to storage location in memory
- **Constants:** an immutable value.

## Declaring Variables / Constants
````csharp
int number;
int Number = 1;
const float PI = 3.14f;
````
### Identifiers
- Cannot start with a number.

````csharp
int 1val; // wrong
int value; // correct
````

- Cannot include whitespaces

````csharp
string first name; // wrong
string firstName; // correct
````

- Connot contain reserved keywords

````csharp
string int; // wrong
string @int; //correct
````

- Use meaningful names
````csharp
string a; // wrong
string age; // correct
````

### Naming Conventions
 - Camel case: **firstName**
 - Pascal case: **FirstName**
 - Hungarian case: **strFirstName**

 ## Primitive Types
 | C# Type        | .NET Type           | Bytes | Ranges |
| ------------- |:-------------:| -----:|:-----:|:------:|
| **byte**      | Byte                  | 1      | 0 to 255             |
| **short**     | Int16                 | 2      | -32,768 to 32,768    |
| **int**       | Int32                 | 4      | -2.1B to 2.1B
| **long**      | Int64                 | 8      | ...
| **float**     | Single                | 4      | -3.4 x 10^28 to 3.4 x 10^28
| **double**    | Double                | 8      | ...
| **decimal**   | Decimal               | 16     | -7.9 x 10^28 to 7.9 x 10^28
| **char**      | Char                  | 2      | Unicode Characters
| **bool**      | Boolean               | 1      | true or false

### Non-primitive types
- String
- Array
- Enum
- Class