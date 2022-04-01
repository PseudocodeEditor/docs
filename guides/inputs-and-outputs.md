---
description: Introduction to Inputting and Outputting Data
---

# Inputs and Outputs

{% hint style="info" %}
This section will take you through basic inputting and outputting of data in Pseudonaja.
{% endhint %}

### Inputs

To input values, the INPUT command is used, however the variable that is being input into must first be declared, as follows:

```
DECLARE <variable name> : <data type>

INPUT <variable name>
```

An example of this would be:

```
DECLARE num1 : INTEGER

INPUT num1
```

### Outputs

To output values, the OUTPUT command is used, as follows:

```
OUTPUT <value>
```

Multiple values can be output at the same time by using commas between each value.

```
OUTPUT <value1>, <value2>, <value3>
```

An example of a single output would be:

```
OUTPUT num1
```

Or multiple outputs:

```
OUTPUT num1, num2, num3
```
