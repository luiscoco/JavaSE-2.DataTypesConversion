# JavaSE-2.DataTypesConversion

In Java, data type conversion can be broadly classified into two types: implicit (automatic) conversion and explicit (manual) conversion. 

Let's go through some examples:

## 1. Implicit Conversion

### 1.1. Widening Primitive Conversion

This happens when you're converting a smaller data type to a larger one.

```java
int intValue = 10;
long longValue = intValue; // Implicit conversion (int to long)
```

### 1.2. Widening Reference Conversion:

In the case of object types, if you're converting from a subclass type to a superclass type.

```java
class Animal { }
class Dog extends Animal { }

Dog myDog = new Dog();
Animal myAnimal = myDog; // Implicit conversion (Dog to Animal)
```

## 2. Explicit Conversion

### 2.1. Narrowing Primitive Conversion

This happens when you're converting a larger data type to a smaller one. You need to explicitly cast.

```java
double doubleValue = 10.5;
int intValue = (int) doubleValue; // Explicit conversion (double to int)
```

### 2.2. Narrowing Reference Conversion:

In the case of object types, if you're converting from a superclass type to a subclass type, you need to explicitly cast.

```java
Animal myAnimal = new Dog();
Dog myDog = (Dog) myAnimal; // Explicit conversion (Animal to Dog)
```

Remember that narrowing conversions may result in loss of data or precision. 
Always be cautious when performing explicit conversions, and make sure the values are within the valid range to avoid unexpected behavior or errors.
