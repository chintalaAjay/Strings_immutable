# Why Strings Are Immutable in Java

This repository demonstrates the concept of **String Immutability in Java** using practical examples with `String` and `StringBuilder`.

---

## What is Immutability?

An immutable object is an object whose value cannot be changed after creation.

In Java, `String` objects are immutable.

---

## Java Program

```java
public class immutablestring {

    public static void main(String[] args) {

        String str = "hello";

        str.concat("world");

        System.out.println(str);

        StringBuilder sb = new StringBuilder("hello");

        sb.append("world");

        System.out.println(sb);

        // correct way to append string

        String str1 = "hello";

        str1 = str1.concat("world");

        System.out.println(str1);
    }
}
Output
hello
helloworld
helloworld



##Explanation
1. String Immutability
String str = "hello";

str.concat("world");

concat() creates a new string object, but the result is not stored.

So original string remains unchanged.

Output:

hello
2. Mutable String Using StringBuilder
StringBuilder sb = new StringBuilder("hello");

sb.append("world");

StringBuilder modifies the same object directly.

Output:

helloworld
3. Correct Way to Modify String
str1 = str1.concat("world");

Here the newly created string is reassigned back to str1.

Output:

helloworld
Why Strings Are Immutable in Java?

Java made strings immutable because of:

Security
Thread Safety
String Pool Optimization
Efficient Hashing
Better Performance
Difference Between String and StringBuilder
Feature	String	StringBuilder
Mutable	❌ No	✅ Yes
Memory Efficient for Modifications	❌	✅
Thread Safe	✅	❌
Performance in Repeated Modifications	Slower	Faster
Concepts Used
String
StringBuilder
Immutability
concat()
append()
Learning Outcome

Through this program, I practiced:

Understanding immutable objects
Difference between String and StringBuilder
Memory behavior in Java strings
String manipulation techniques

⭐ Learning Java concepts deeply through practical coding examples.
