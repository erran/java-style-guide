# Java Style Guide
My personal Java coding style guide. These are standards I've learned from
different sources and want to convert into a format similar to the Ruby
style guide's.

## Table of Contents
* [Source Code Layout](#source-code-layout)
* [Classes](#classes)

## Source Code Layout
* Use three **spaces** (soft tabs) per indentation level.
* Adopt a consistent brace-line style. There are two popular styles in the
Java community both of which are considered good - trailing braces (Option A) and leading braces (Option B).
  * **(Option A)** Braces on the same line as the previous expression.
    ```java
    // bad - can be unclear when using throws/extends/implements
    // on class/method definitions
    if (isOdd()) {
    }

    // good - works naturally with throws/extends/implements
    if (isEven())
    {
    }
    ```
  * **(Option B)** Braces on the subsequent line.
    ```java
    // bad - adds extra insignificant lines
    if (isOdd())
    {
    }

    // good - reduces the LOC (lines of code)
    if (isEven()) {
    }
    ```

# Classes
* Use a consistent structure in your class definitions.

 ```java
 public class Car
 {
    // public constructors
    public Car(String make, String model)
    {
       m_make = make;
       m_model = model;
    }

    // public methods
    public String toString()
    {
       return getMakeString() + " model: " + m_model;
    }

    // protected/private methods
    private String getMakeString()
    {
       return "make: " + m_make;
    }

    // protected/private members
    private String m_make;
    private String m_model;

    // protected/private static members
    private static Logger ms_logger; 
 }
 ```
