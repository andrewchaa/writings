programming in java in 10 years
=====================

I learned java at Uni. and worked really hard. Yet, I didn't have chance to use it when I becaue a full time programmer.
I was a Delphi and VB guy and then C# man. I didn't plan it, but it turned out that my career was more oriented toward Microsoft Stack.

And, now I'm reading [TDD By Example](http://www.amazon.co.uk/Driven-Development-Addison-Wesley-Signature-Series/dp/0321146530/ref=sr_1_1?ie=UTF8&qid=1344332680&sr=8-1). 
This is my third read, and I thought it might be fun to try the examples in java. Previously, I converted those examples to C# code. 
So, this is my experience with java.

Java IDE
--------------------

You need an ide to code. as I am a loyal ReSharper user, my first choic was IntelliJ. It was funny, that most of things I loved about ReSharper, actually came from IntelliJ.
[Community Edition](http://www.jetbrains.com/idea/download/) is free. 


Hello World
--------------------

Writing "Hello, World!" is a challenge, if you do not know the eco-system of the language. Java syntax is very similar to C#, yet I didn't know how to write a simple console application. jetbrains' wiki had a nice tutorial about [how to create the first java application](http://wiki.jetbrains.net/intellij/Creating_and_running_your_first_Java_application).

This is my code, nothing clever or unusual.

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

Now, next challenge is to write the first unit test. I have no idea how to add junit. I wanted to trust IntelliJ and added @Test attribute (not sure if this is called attribute) and used "Press Alt + ENTER" that works for all. And it added junit-4.10.jar to external libraries. Also, it's interesting that import works like "org.junit.Assert.*" I thought by specifying "org.junit.Assert", all methods that belong to Assert would come, but I had to use *. It's different from C#'s name space. [JUnitQuickTutorial](http://code.google.com/p/t2framework/wiki/JUnitQuickTutorial) helped me to get started.


```java

package com.example.helloworld;

import org.junit.Test;
import static org.junit.Assert.*;

/**
 * Created with IntelliJ IDEA.
 * User: andrew.chaa
 * Date: 07/08/12
 * Time: 11:12
 * To change this template use File | Settings | File Templates.
 */
public class HelloWorldTest {
    @Test
    public void test_true() {
        assertTrue(true);
    }
}

```

