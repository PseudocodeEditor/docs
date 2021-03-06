---
description: Introduction to Declaring Variables and Arrays in Pseudonaja
---

# Declaring Variables and Arrays

{% hint style="info" %}
This guide is going to take you through the process of basic declaration of variables in Pseudonaja.
{% endhint %}

### Basic Variables

To use variables in Pseudonaja we first need to declare the variable. This can be done using the following command:

```
DECLARE <variable name> : <data type>
```

An example of this is:

```
DECLARE num1 : INTEGER
```

{% hint style="info" %}
You can also use commas to DECLARE multiple variables
{% endhint %}

```
DECLARE num1, num2, num3 : INTEGER
```

Available data types:

| Datatype Command | Type                                               |
| ---------------- | -------------------------------------------------- |
| INTEGER          | A single integer number                            |
| REAL             | A single float / real number                       |
| BOOLEAN          | A binary TRUE or FALSE value                       |
| CHAR             | A single character                                 |
| STRING           | A string of multiple characters                    |
| ARRAY            | An array of fixed length of a particular data type |

{% hint style="warning" %}
To assign a value to a variable, instead of an = sign, an <- is used instead, after the variable has been declared.
{% endhint %}

```
num1 <- 3
```

### Arrays

In pseudocode you declare arrays slightly differently:

```
DECLARE <array name> : ARRAY [<lower bound>:<upper bound>] OF <data type>
```

An example of this is:

```
DECLARE myArray : ARRAY[0:100] OF INTEGER
```

{% hint style="warning" %}
Unlike lists in python arrays can only consist of a single data type as well as a fixed length.
{% endhint %}

**Two dimensional arrays** are declared as follows:

```
DECLARE <array name> ARRAY [<1ower bound 1>:<upper bound 1>, <1ower bound 1>:<upper bound 2>] OF <data type>
```

An example of this is:

```
DECLARE my2DArray ARRAY [0:100, 0:1] OF CHAR
```

#### Accessing Arrays

To access a 1D array:

```
DECLARE myArray : ARRAY[0:100] OF INTEGER

myArray[19] <- 29
```

To access a 2D array:

```
DECLARE my2DArray ARRAY [0:100, 0:1] OF CHAR

my2DArray[12, 1] <- 'B'
```

Where the first value within the assignment statement is the row to be accessed, and the second value is the column to be accessed. &#x20;
