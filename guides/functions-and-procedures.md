---
description: Introduction to Functions and Procedures
---

# Functions and Procedures

### Functions

Functions are algorithms that can be called to execute an already written set of code, and return a value to where they were called. They use the keywords FUNCTION, RETURNS, ENDFUNCTION. Functions can be used either with or without parameters.

```
FUNCTION <function name> RETURNS <data type to return>
    <code to be executed>
ENDFUNCTION
```

Alternatively, with parameters:

```
FUNCTION <function name>(<parameter1> : <data type>,
                         <parameter2> : <data type>...)
                         RETURNS <data type to return>
    <code to be executed>
ENDFUNCTION
```

The keyword RETURN is used to specify a value to be returned within the function. Upon encountering a RETURN statement, it is executed immediately, and any lines after the statement are ignored.

```
FUNCTION Add(num1 : INTEGER, num2 : INTEGER) RETURNS INTEGER
    num3 <- num1 + num2
    RETURN num3
ENDFUNCTION
```

### Procedures

Procedures are similar to functions, however they do not return any value. They use the keywords PROCEDURE, ENDPROCEDURE. Procedures can also be used with or without parameters.

```
PROCEDURE <procedure name>
    <code to be executed>
ENDPROCEDURE
```

With parameters:

```
PROCEDURE <procedure name>(<parameter1> : <data type>, 
                           <parameter2> : <data type>...)
    <code to be executed>
ENDPROCEDURE
```

Procedures must be called using the CALL keyword, used respectively as follows:

```
CALL <procedure name>
```

```
CALL <procedure name>(<parameter1>, <parameter2>, ...)
```

An example of procedure definition and calling:

```
PROCEDURE Add(num1 : INTEGER, num2 : INTEGER)
    num3 <- num1 + num2
    OUTPUT num3
ENDPROCEDURE

CALL Add(10, 5)
```
