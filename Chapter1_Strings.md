## Understanding `String`

- **Immutable**: Once a `String` object is created, it cannot be changed. Any modification to a `String` results in the creation of a new `String` object.
- **Usage**: Ideal for scenarios where the string content does not change frequently.

### Example
```java
String str = "Hello";
str = str + " World"; // Creates a new String object
