# Type conversion
- Implicit type conversion
- Explicit type conversion (casting)
- Conversion between non-compatible types

## Implicit type conversion

````csharp
byte b = 1; //                            00000001
int i = b;  // 00000000 00000000 00000000 00000001
````

## Explicit type conversion

````csharp
int i = 1;
byte b = i; // won't compile

byte c = (byte)i; // correct way to handle explicit coversions

// another example
float f = 1.0f;
int i = (int)f;

````

## Non-compatible types conversion

````csharp
string s = "1";

int i = (int)s; // won't compile

// the correct way to handle non-compatible type conversion
string s1 = "1";

int i1 = Convert.ToInt32(s);
int j = int.Parse(s);

````

## Methods inside Convert class
- ToByte()
- ToInt16()
- ToInt32()
- ToInt64()