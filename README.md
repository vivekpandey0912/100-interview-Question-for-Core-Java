Here are 100 Java interview questions along with their answers. These questions cover various topics related to Java programming and are commonly asked during interviews:

1. What is Java?
   Java is a high-level, object-oriented programming language developed by Sun Microsystems (now owned by Oracle). It is designed to be platform-independent, allowing developers to write code once and run it on any platform that has a Java Virtual Machine (JVM).

2. What are the main features of Java?
   Main features of Java include:
   - Object-oriented
   - Platform-independent
   - Robust and secure
   - Multithreaded
   - Simple and familiar syntax
   - Automatic memory management (Garbage Collection)

3. Explain the difference between JDK, JRE, and JVM.
   - JDK (Java Development Kit): It includes tools like the compiler and debugger necessary for Java development.
   - JRE (Java Runtime Environment): It contains the JVM, along with the libraries and other resources required to run Java applications.
   - JVM (Java Virtual Machine): It is the runtime environment in which Java bytecode is executed.

4. What is the difference between `==` and `.equals()` in Java?
   - `==` is used to compare primitive data types and object references (memory addresses).
   - `.equals()` is a method used to compare the contents of objects for equality. It is typically overridden by classes to provide meaningful comparisons.

5. What is the difference between the stack and the heap in Java memory management?
   - Stack: It is used for storing method call frames and local variables. It operates in a Last-In-First-Out (LIFO) manner.
   - Heap: It is used for dynamically allocated memory for objects. Objects in the heap can be accessed from multiple methods or threads.

6. How do you create an object in Java?
   To create an object in Java, you use the `new` keyword followed by the class constructor. For example:
   ```
   MyClass obj = new MyClass();
   ```

7. What are constructors in Java?
   Constructors are special methods in a class used to initialize object instances. They have the same name as the class and are called when an object is created using the `new` keyword.

8. Can a constructor be private in Java?
   Yes, a constructor can be made private in Java. A private constructor is typically used to prevent the instantiation of a class from outside the class itself.

9. What is method overloading in Java?
   Method overloading allows a class to have multiple methods with the same name but different parameter lists. The methods are differentiated based on the number or types of arguments they accept.

10. What is method overriding in Java?
    Method overriding allows a subclass to provide a specific implementation for a method that is already defined in its superclass. The method signature in the subclass must exactly match the method in the superclass.

11. What are access modifiers in Java? Explain them.
    Access modifiers in Java control the visibility and accessibility of class members (variables, methods, constructors). There are four types:
    - `public`: The member is accessible from any class.
    - `protected`: The member is accessible within the same package and subclasses.
    - `default` (no modifier): The member is accessible only within the same package.
    - `private`: The member is accessible only within the same class.

12. What is the final keyword in Java?
    The `final` keyword can be used with classes, methods, and variables.
    - Final class: A class declared as final cannot be subclassed.
    - Final method: A method declared as final cannot be overridden by subclasses.
    - Final variable: A variable declared as final cannot be reassigned once initialized.

13. Can the main() method be made final in Java?
    No, the main() method cannot be made final in Java. The JVM requires an entry point with a specific signature, and making it final would prevent the JVM from accessing it.

14. What are static variables and methods in Java?
    - Static variables: They belong to the class rather than an instance of the class. All instances of the class share the same static variable.
    - Static methods: They are associated with the class and not with any specific instance. They can be called using the class name without creating an object.

15. What is the difference between static and non-static (instance) variables/methods?
    - Static variables/methods belong to the class itself, while non-static variables/methods belong to instances of the class.
    - Static variables/methods are accessed using the class name, while non-static variables/methods are accessed using the object reference.

16. Can you call a non-static method from a static method in Java?
    Yes, you can call a non-static method from a static method, but you need to create an instance of the class to call the non-static method.

17. What is the `this` keyword in Java?
    `this` is a reference to the current instance of the class. It is used to differentiate between instance variables and method parameters that have the same name.

18. What is a package in Java?
    A package is a way to organize classes and interfaces into different namespaces to avoid naming conflicts. It helps in creating a modular and hierarchical structure for Java applications.

19. How do you import classes from another package in Java?
    To import classes from another package, you use the `import` statement at the beginning of your Java file. For example:
    ```
    import java.util.ArrayList;
    ```

20. What is an interface in Java?
    An interface is a collection of abstract methods and constant variables. It defines a contract that classes must implement if they want to be considered of that interface type.

21. Can you create an object of an interface in Java?
    No, you cannot create an object of an interface directly. However, you can create an instance of a class that implements the interface and use that to access the interface methods.

22. What is the difference between abstract classes and interfaces in Java?
    - Abstract classes can have both abstract and concrete methods, while interfaces can only have abstract methods (prior to Java 8).
    - A class can implement multiple interfaces, but it can extend only one abstract class.

23. What are lambda expressions in Java 8?
    Lambda expressions provide a concise way to represent a single-method interface (functional interface). They allow you to treat functionality as a method argument.

24. What is the use of the `static` block in Java?
    The `static` block is used to initialize static variables or perform some static setup tasks when the class is loaded by the JVM. It runs only once when the class is initialized.

25. What is the purpose of the `final` block in Java exception handling?
    The `final` block is used in conjunction with `try-catch` blocks. It contains code that will always be executed, regardless of whether an exception occurs or not.

26. What is the difference between checked and unchecked exceptions in Java?
    - Checked exceptions: These are exceptions that need to be either caught and handled using `try-catch` or declared in the method signature using `throws`.
    - Unchecked exceptions: Also known as runtime exceptions, these do not need to be declared or handled explicitly. They are subclasses of `RuntimeException`.

27. What is a try-with-resources statement in Java?
    The try-with-resources statement is used to automatically close resources (such as file streams or network

 connections) after their operations are complete. It simplifies resource management.

28. What is the `StringBuilder` class in Java? How is it different from `String`?
    `StringBuilder` is a mutable sequence of characters, while `String` is immutable. `StringBuilder` is more efficient when frequent modifications are needed, as it avoids creating new objects for each change.

29. What is the `hashCode()` method in Java?
    The `hashCode()` method returns a hash code value for an object. It is used for hashing-based data structures like HashMap and HashSet to efficiently locate objects.

30. What is the purpose of the `equals()` method in Java?
    The `equals()` method is used to compare the content of objects for equality. It is used in conjunction with the `hashCode()` method when dealing with collections like HashMap and HashSet.

31. Can you compare strings in Java using the `==` operator?
    While `==` compares object references, it does not compare the content of strings. To compare the content of strings, you should use the `.equals()` method.

32. What is the `StringBuffer` class in Java? How is it different from `StringBuilder` and `String`?
    `StringBuffer` is similar to `StringBuilder`, but it is synchronized (thread-safe). It is used in multi-threaded environments where multiple threads may access the same `StringBuffer` instance.

33. What are anonymous classes in Java?
    Anonymous classes are classes without names that can be defined and instantiated in a single expression. They are often used to implement interfaces or extend classes without explicitly creating a new class.

34. What is the `instanceof` operator used for in Java?
    The `instanceof` operator is used to check if an object is an instance of a particular class or implements a specific interface. It returns `true` if the object is an instance of the specified type; otherwise, it returns `false`.

35. How does Java handle multiple inheritance?
    Java does not support multiple inheritance through classes (i.e., a class cannot extend multiple classes). However, it allows multiple inheritance through interfaces, where a class can implement multiple interfaces.

36. What is the Java Memory Model (JMM)?
    The Java Memory Model defines how the threads in a Java program interact through memory. It ensures that the changes made by one thread are visible to other threads in a consistent manner.

37. What are threads in Java, and how are they created?
    Threads are lightweight processes that allow concurrent execution in Java. Threads can be created in two ways:
    - By extending the `Thread` class and overriding the `run()` method.
    - By implementing the `Runnable` interface and passing it to a `Thread` constructor.

38. How do you start a thread in Java?
    To start a thread, you call the `start()` method on the `Thread` object. This method internally calls the `run()` method of the thread.

39. What is synchronization in Java, and why is it used?
    Synchronization is used to ensure that only one thread can access a shared resource at a time. It prevents data inconsistency and race conditions that can occur when multiple threads access the same resource concurrently.

40. What are synchronized methods and synchronized blocks in Java?
    - Synchronized methods: These are methods that are declared with the `synchronized` keyword. Only one thread can execute a synchronized method at a time.
    - Synchronized blocks: These are blocks of code enclosed within `synchronized` statements. They allow fine-grained control over the portion of code that needs synchronization.

41. What is a deadlock in Java?
    Deadlock occurs when two or more threads are blocked, each waiting for a resource that another thread in the set holds. This can lead to a situation where all the threads are indefinitely waiting for resources, and the application stops responding.

42. How can you prevent deadlock in Java?
    Deadlock can be prevented by ensuring that threads always request resources in the same order. Additionally, you can use timeout mechanisms, employ lock hierarchies, or use the `java.util.concurrent` package for higher-level synchronization constructs.

43. What is the `volatile` keyword in Java?
    The `volatile` keyword is used to mark a variable as not subject to thread caching. When a variable is marked as `volatile`, any read or write operation on that variable will be done directly from/to the main memory, ensuring visibility to all threads.

44. What is the purpose of the `transient` keyword in Java?
    The `transient` keyword is used to indicate that a field should not be serialized when an object is converted to a byte stream (e.g., during object serialization).

45. What is the `serialVersionUID` in Java serialization?
    The `serialVersionUID` is a unique identifier used during object serialization to ensure that the serialized and deserialized objects are compatible. If not provided explicitly, Java computes it based on the class definition.

46. How do you handle exceptions in multi-threaded environments?
    In multi-threaded environments, exceptions should be caught and handled within each thread separately. If an exception is not caught within a thread, it can cause the thread to terminate, affecting the entire application's stability.

47. What is a lambda function?
    A lambda function is a concise way to represent an anonymous function, also known as a lambda expression. It allows the implementation of functional interfaces in a more readable and less verbose way.

48. What are the different ways to create threads in Java 8 or later versions?
    In Java 8 and later, you can create threads using lambda expressions, method references, or by using the new `CompletableFuture` API for asynchronous programming.

49. What is the purpose of the `CompletableFuture` class in Java 8?
    `CompletableFuture` is used for asynchronous programming in Java 8 and later versions. It represents a computation that may complete in the future, and you can chain various operations on it, making it easier to write concurrent code.

50. How does garbage collection work in Java?
    Garbage collection in Java is an automatic process that reclaims memory occupied by objects that are no longer in use or reachable. The JVM identifies unused objects and releases their memory to be reused.

51. What is the `finalize()` method in Java?
    The `finalize()` method is a method in the `Object` class, which all objects inherit. It is called by the garbage collector before an object is garbage collected, allowing you to perform cleanup operations.

52. What is the difference between `finalize()` and `dispose()` methods in Java?
    - `finalize()`: It is a method called by the garbage collector before an object is reclaimed.
    - `dispose()`: It is a convention used in some classes to perform cleanup operations before an object is no longer needed. It is not a standard method like `finalize()`.

53. How can you force garbage collection in Java?
    In Java, you can request garbage collection by calling `System.gc()` or `Runtime.getRuntime().gc()`. However, it does not guarantee immediate garbage collection; the JVM may choose to ignore the request.

54. How is the `ArrayList` different from the `LinkedList` in Java?
    - `ArrayList`: It is a dynamic array implementation, where elements are stored in a contiguous block of memory. It provides fast random access but slower insertion and deletion in the middle.
    - `LinkedList`: It is a linked list implementation, where elements are stored in separate nodes

 connected by pointers. It provides fast insertion and deletion in the middle but slower random access.

55. What is the difference between `Iterator` and `ListIterator` in Java?
    - `Iterator`: It is used to iterate over a collection in a unidirectional manner (forward only).
    - `ListIterator`: It extends `Iterator` and allows bidirectional traversal (forward and backward) of a list. It is specific to lists and not available for all collections.

56. What is the `Comparable` interface in Java?
    The `Comparable` interface is used to impose a natural ordering on a class. Classes that implement this interface can be sorted using `Arrays.sort()` or `Collections.sort()`.

57. What is the `Comparator` interface in Java?
    The `Comparator` interface is used to impose an external ordering on a class. It allows you to sort objects based on different criteria without modifying their original implementation.

58. What is the purpose of the `java.lang` package in Java?
    The `java.lang` package contains fundamental classes and is automatically imported into all Java programs. It provides essential classes like `Object`, `String`, and basic data types.

59. How do you handle ConcurrentModificationException in Java?
    ConcurrentModificationException occurs when a collection is modified while being iterated using an iterator. To avoid this, use `Iterator` or enhanced for loop instead of directly modifying the collection.

60. What is the Java `ClassLoader`? How does it work?
    The `ClassLoader` is responsible for loading classes into the JVM. It follows a hierarchical order (bootstrap class loader, extension class loader, and application class loader) to find and load classes.

61. How do you create and use a custom exception in Java?
    To create a custom exception, you need to create a class that extends the `Exception` or a subclass of it. Use the `throw` keyword to throw the custom exception when needed.

62. What is the `assert` keyword in Java?
    The `assert` keyword is used for debugging and testing purposes. It checks a condition and throws an `AssertionError` if the condition is false. Assertion checking is typically disabled in production code.

63. What are annotations in Java? Provide examples of built-in annotations.
    Annotations are metadata added to Java classes, methods, fields, or other elements. They provide additional information to the compiler or runtime. Examples of built-in annotations are `@Override`, `@Deprecated`, and `@SuppressWarnings`.

64. What is reflection in Java? How can you use it?
    Reflection allows you to inspect and manipulate classes, interfaces, methods, and fields at runtime. You can access class information, invoke methods, and create instances dynamically using reflection.

65. What is the purpose of the `java.lang.Object` class in Java?
    The `java.lang.Object` class is the root of the class hierarchy in Java. All classes implicitly or explicitly extend this class. It provides essential methods like `equals()`, `hashCode()`, and `toString()`.

66. What is the difference between shallow copy and deep copy in Java?
    - Shallow copy: It creates a new object and copies the references of the original object's fields. Both the original and copied objects share the same referenced objects.
    - Deep copy: It creates a new object and copies all the referenced objects recursively. The copied object is completely independent of the original object.

67. How can you create a shallow copy and deep copy of an object in Java?
    To create a shallow copy, you can use the `clone()` method, if the class implements the `Cloneable` interface. For a deep copy, you need to create a custom method that performs a deep copy recursively.

68. How does Java handle integer division?
    In Java, integer division truncates the decimal part, returning only the integer part of the result. For example, `5 / 2` returns `2`, not `2.5`.

69. What is autoboxing and unboxing in Java?
    - Autoboxing: It is the process of automatically converting primitive data types into their corresponding wrapper classes (e.g., `int` to `Integer`).
    - Unboxing: It is the process of automatically converting wrapper classes back to their primitive data types.

70. What are varargs in Java?
    Varargs (variable-length arguments) allow methods to accept an arbitrary number of arguments of the same type. They are declared using an ellipsis (`...`) followed by the type of arguments.

71. How do you handle OutOfMemoryError in Java?
    OutOfMemoryError occurs when the JVM runs out of memory due to excessive object creation or insufficient memory allocation. You can handle it by analyzing your application for memory leaks, increasing heap size, or optimizing memory usage.

72. How do you convert a string to an integer in Java?
    You can convert a string to an integer using the `Integer.parseInt()` or `Integer.valueOf()` methods:
    ```
    String str = "123";
    int num1 = Integer.parseInt(str);   // Using parseInt()
    Integer num2 = Integer.valueOf(str); // Using valueOf()
    ```

73. How do you convert an integer to a string in Java?
    You can convert an integer to a string using the `String.valueOf()` method or by using concatenation with an empty string:
    ```
    int num = 123;
    String str1 = String.valueOf(num);   // Using valueOf()
    String str2 = num + "";              // Using concatenation
    ```

74. How can you generate a random number in Java?
    To generate a random number in Java, you can use the `Random` class from the `java.util` package or the `Math.random()` method.
    ```
    Random random = new Random();
    int randomNumber = random.nextInt(100); // Generates a random number between 0 and 99

    double randomDouble = Math.random();    // Generates a random double between 0.0 (inclusive) and 1.0 (exclusive)
    ```

75. What is the `Math` class in Java, and how is it used

?
    The `Math` class in Java provides mathematical functions and constants. It contains methods like `sqrt()`, `pow()`, `cos()`, `sin()`, etc. You can use these methods to perform various mathematical calculations.

76. What is a `static` initializer block in Java?
    A static initializer block is a block of code enclosed in curly braces and marked with the `static` keyword. It is executed when the class is loaded by the JVM and runs before the class constructor.

77. How do you reverse a string in Java?
    You can reverse a string in Java using various methods. One common approach is to convert the string to a character array, then reverse the array, and finally convert it back to a string.
    ```
    String original = "Hello";
    char[] chars = original.toCharArray();

    int start = 0;
    int end = chars.length - 1;
    while (start < end) {
        char temp = chars[start];
        chars[start] = chars[end];
        chars[end] = temp;
        start++;
        end--;
    }

    String reversed = new String(chars);
    System.out.println(reversed); // Output: "olleH"
    ```

78. What is the `System.arraycopy()` method used for in Java?
    The `System.arraycopy()` method is used to efficiently copy elements from one array to another. It provides a faster way to copy arrays than using loops.

79. How do you find the length of an array in Java?
    To find the length of an array in Java, you can use the `length` property:
    ```
    int[] numbers = {1, 2, 3, 4, 5};
    int length = numbers.length; // length is 5
    ```

80. How do you find the maximum and minimum values in an array in Java?
    You can find the maximum and minimum values in an array by iterating through the array and keeping track of the maximum and minimum values found so far.
    ```
    int[] numbers = {10, 5, 8, 12, 3};
    int max = numbers[0];
    int min = numbers[0];

    for (int i = 1; i < numbers.length; i++) {
        if (numbers[i] > max) {
            max = numbers[i];
        }
        if (numbers[i] < min) {
            min = numbers[i];
        }
    }

    System.out.println("Max: " + max); // Output: "Max: 12"
    System.out.println("Min: " + min); // Output: "Min: 3"
    ```

81. What is the `TreeSet` class in Java?
    `TreeSet` is an implementation of the `Set` interface that uses a self-balancing binary search tree (Red-Black Tree) to store elements. It maintains elements in sorted order.

82. What is the `HashSet` class in Java?
    `HashSet` is an implementation of the `Set` interface that uses a hash table to store elements. It does not maintain elements in any specific order.

83. What is the `LinkedHashSet` class in Java?
    `LinkedHashSet` is an implementation of the `Set` interface that maintains elements in insertion order (order of insertion).

84. What is the `HashMap` class in Java?
    `HashMap` is an implementation of the `Map` interface that uses a hash table to store key-value pairs. It allows rapid retrieval of values based on keys.

85. What is the `LinkedHashMap` class in Java?
    `LinkedHashMap` is an implementation of the `Map` interface that maintains the order of elements based on their insertion order.

86. What is the `TreeMap` class in Java?
    `TreeMap` is an implementation of the `Map` interface that stores keys in sorted order (ascending by default). It uses a Red-Black Tree to maintain the keys in sorted order.

87. What is the difference between `HashMap` and `Hashtable` in Java?
    - `HashMap`: It is not synchronized and allows `null` keys and values. It is generally preferred for single-threaded applications.
    - `Hashtable`: It is synchronized and does not allow `null` keys or values. It is considered legacy and has been largely replaced by `HashMap` or `ConcurrentHashMap`.

88. What is the `Collections` class in Java?
    The `Collections` class is a utility class in Java that provides various methods for working with collections, such as sorting, searching, and manipulation.

89. What is the `Arrays` class in Java?
    The `Arrays` class is a utility class in Java that provides various methods for working with arrays, such as sorting, searching, and filling.

90. What is the purpose of the `java.util` package in Java?
    The `java.util` package provides utility classes and interfaces for collections, date and time, random number generation, and other common tasks.

91. What are the advantages of using Java over other programming languages?
    - Platform independence: Java programs can run on any platform with a Java Virtual Machine (JVM).
    - Object-oriented: Java follows object-oriented programming principles, making it easy to model real-world entities.
    - Rich API: Java has a vast standard library (API) for various tasks, simplifying development.
    - Memory management: Java uses automatic garbage collection, reducing the burden on developers.
    - Multithreading: Java supports concurrent programming, enabling applications to execute multiple tasks simultaneously.



92. What is the `volatile` keyword used for in Java?
    The `volatile` keyword is used to indicate that a variable's value may be modified by multiple threads. It ensures that changes to the variable are visible to all threads.

93. What is the difference between the `finalize()` method and the `finally` block in Java?
    - `finalize()`: It is a method in the `Object` class that is called by the garbage collector before reclaiming an object's memory.
    - `finally`: It is a block used in conjunction with `try-catch` to ensure that a block of code (e.g., resource cleanup) always executes, regardless of whether an exception is thrown or not.

94. How do you implement a multi-threaded server in Java?
    To implement a multi-threaded server in Java, you can use the `java.net` package to handle client connections. Each client connection is handled by a separate thread to allow concurrent processing.

95. How can you handle concurrency issues in multi-threaded Java applications?
    Concurrency issues in multi-threaded Java applications can be handled using synchronization mechanisms like `synchronized` blocks, locks, and concurrent collections from `java.util.concurrent` package.

96. What are the different types of class loaders in Java?
    There are three types of class loaders in Java:
    - Bootstrap class loader: Loads core Java classes from the system classpath.
    - Extension class loader: Loads classes from the extension classpath.
    - Application class loader: Loads classes from the application classpath.

97. How do you perform input/output (I/O) operations in Java?
    Java provides various classes in the `java.io` package for performing I/O operations. For example, you can use `FileInputStream`, `FileOutputStream`, `BufferedReader`, `BufferedWriter`, etc., for reading and writing files.

98. What are the different types of streams in Java I/O?
    There are two types of streams in Java I/O:
    - Byte streams: Used for handling binary data, like reading and writing bytes from/to files.
    - Character streams: Used for handling character-based data, like reading and writing characters from/to files. They are typically used for text-based I/O.

99. What is the `try-with-resources` statement in Java I/O?
    The `try-with-resources` statement is used to automatically close resources (like files) after their operations are complete. It ensures that resources are released properly, even if an exception occurs.

100. How do you handle file operations in Java, such as reading and writing files?
    In Java, you can use classes like `File`, `FileInputStream`, `FileOutputStream`, `BufferedReader`, and `BufferedWriter` to perform file-related operations. You open a file, read or write data, and close the file using `try-with-resources` to handle resources properly.
