# Java Style Guide
My personal Java coding style guide. These are standards I've learned from
different sources and want to convert into a format similar to the Ruby
style guide's.

## Table of Contents
* [Source Code Layout](#source-code-layout)

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