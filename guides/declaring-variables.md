---
description: Introduction to Declaring Variables in Pseudonaja
---

# Declaring Variables

{% hint style="info" %}
This guide is going to take you throught the process of basic declaration of variables in pseudonaja.
{% endhint %}

### Basic Variables

To use variables in pseudonaja we first need to decalre the variable. This can be done using the following command:

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

| Datatype Command | Type                                               | Notes           |
| ---------------- | -------------------------------------------------- | --------------- |
| INTEGER          | A single integer number                            |                 |
| REAL             | A single float / real number                       |                 |
| BOOLEAN          | A binary TRUE or FALSE value                       |                 |
| CHAR             | A single character                                 |                 |
| STRING           | A string of multiple characters                    |                 |
| ARRAY            | An array of fixed length of a particular data type | See notes below |

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
Unlike lists in python arrays can only consist of a single data type.
{% endhint %}

**Two dimensional arrays** are declared as follows:

```
DECLARE <array name> ARRAY [<1ower bound 1>:<upper bound 1>, <1ower bound 1>:<upper bound 2>] OF <data type>
```

An example of this:

```
DECLARE my2DArray ARRAY [0:100, 0:1] OF CHAR
```
