### 1. **`extends`**

**Purpose**: Indicates that a class is inheriting from another class (i.e., it is a child class or subclass).

**Usage**: Used with classes to implement inheritance.

**Example**:
```java
class Animal {
    // Parent class
}

class Dog extends Animal {
    // Child class, inherits from Animal
}
```
---

### 2. **`implements`**


# `implements`

**Purpose**: Indicates that a class is implementing an interface (i.e., providing concrete implementations for the methods defined in the interface).

**Usage**: Used with classes to implement interfaces.

**Example**:
```java
interface AnimalBehavior {
    void makeSound();
}

class Dog implements AnimalBehavior {
    public void makeSound() {
        System.out.println("Bark");
    }
}
```
---

### 3. **`abstract`**

```md
# `abstract`

**Purpose**: Used to declare a class as abstract, meaning it cannot be instantiated and is meant to be subclassed. It can also be used to declare abstract methods within a class that must be implemented by subclasses.

**Usage**: Applied to classes and methods.

**Example**:
```java
abstract class Animal {
    abstract void makeSound(); // Abstract method
}

class Dog extends Animal {
    void makeSound() {
        System.out.println("Bark");
    }
}
```
---

### 4. **`interface`**

```md
# `interface`

**Purpose**: Used to declare an interface, a reference type that can contain abstract methods, default methods, static methods, and final fields. Classes use the `implements` keyword to implement interfaces.

**Usage**: Defines a contract that classes can implement.

**Example**:
```java
interface AnimalBehavior {
    void makeSound();
}

class Dog implements AnimalBehavior {
    public void makeSound() {
        System.out.println("Bark");
    }
}
```
---

### 5. **`super`**

```md
# `super`

**Purpose**: Refers to the superclass (parent class) of the current object. It's used to access superclass methods, constructors, and variables.

**Usage**: Used within a subclass to refer to the parent class's members.

**Example**:
```java
class Animal {
    void makeSound() {
        System.out.println("Animal sound");
    }
}

class Dog extends Animal {
    void makeSound() {
        super.makeSound(); // Calls the parent class method
        System.out.println("Bark");
    }
}
```
---

### 6. **`this`**

```md
# `this`

**Purpose**: Refers to the current instance of the class. It's used to access the class's own fields, methods, and constructors.

**Usage**: Used within a class to differentiate between instance variables and parameters or to call other constructors.

**Example**:
```java
class Dog {
    private String name;

    Dog(String name) {
        this.name = name; // 'this' refers to the current object's name variable
    }

    void printName() {
        System.out.println(this.name);
    }
}
```
---

### 7. **`final`**

```md
# `final`

**Purpose**: Used to declare constants, prevent method overriding, or prevent inheritance of a class.

**Usage**: Applied to variables, methods, and classes.

**Examples**:
- **Variable**: A `final` variable cannot be reassigned.
- **Method**: A `final` method cannot be overridden by subclasses.
- **Class**: A `final` class cannot be subclassed.

```java
final class Animal {
    final void makeSound() {
        System.out.println("Animal sound");
    }
}
```
---

### 8. **`static`**

```md
# `static`

**Purpose**: Used to declare class-level variables and methods, meaning they belong to the class rather than any instance of the class.

**Usage**: Applied to variables, methods, and blocks.

**Example**:
```java
class Animal {
    static int count = 0; // Static variable

    static void incrementCount() { // Static method
        count++;
    }
}
```
---

### 9. **`native`**

```md
# `native`

**Purpose**: Indicates that a method is implemented in native code (e.g., C or C++) rather than in Java.

**Usage**: Used for methods that interact with system-level resources or legacy code.

**Example**:
```java
public class NativeExample {
    public native void nativeMethod(); // Declaration of a native method
}
```
---

### 10. **`synchronized`**

```md
# `synchronized`

**Purpose**: Used to control the access of multiple threads to a block/method of code. It ensures that only one thread can execute the synchronized block/method at a time.

**Usage**: Applied to methods or blocks of code to make them thread-safe.

**Example**:
```java
public synchronized void increment() {
    // Only one thread can execute this at a time
}
```
---

### 11. **`volatile`**

```md
# `volatile`

**Purpose**: Indicates that a variable's value will be modified by different threads. Ensures that the value of the variable is always read from the main memory, not from the thread's local cache.

**Usage**: Applied to variables.

**Example**:
```java
private volatile boolean isRunning = true;
```
---

### 12. **`transient`**

```md
# `transient`

**Purpose**: Prevents serialization of a field in an object. During serialization, the field marked as `transient` will not be serialized.

**Usage**: Applied to instance variables.

**Example**:
```java
class Employee implements Serializable {
    private transient int SSN; // This field won't be serialized
    private String name;
}
