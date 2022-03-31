---
description: Introduction to Conditional Structures
---

# Conditional Structures

In pseudocode, there are two types of conditional structures that are utilised, being IF statements and CASE statements.

### IF Statements

IF statements utilise a specific set of keywords that need to be included, being IF, THEN, ENDIF.

```
IF <condition> THEN
    <code to be executed>
ENDIF
```

E.g:

```
IF num1 = 3 THEN
    OUTPUT "num1 is 3"
ENDIF
```

IF statements can also include an ELSE clause to be able to branch into other code depending on if the IF statement has passed or not.

```
IF <condition> THEN
    <code to be executed>
ELSE
    <code to otherwise be executed>
ENDIF
```

E.g:

```
IF num1 = 3 THEN
    OUTPUT "num1 is 3"
ELSE
    OUTPUT "num1 isn't 3"
ENDIF
```

Nested IF statements can also be used, however, care must be taken with inserting ENDIFs into the correct locations. An example of this would be:

```
IF num1 = 3 THEN
    IF num2 = 3 THEN
        OUTPUT "num1 and num2 are 3"
    ELSE
        OUTPUT "Only num1 is 3"
    ENDIF
ELSE
    IF num2 = 3 THEN
        OUTPUT "Only num2 is 3"
    ELSE
        OUTPUT "Neither num1 or num2 is 3"
    ENDIF
ENDIF
```

### CASE Statements

CASE statements are where multiple branches of code can be executed, depending on the value of the variable given to the statement. They follow the keywords CASE OF, ENDCASE.

```
CASE OF <variable>
    <value1> : <code to be executed>
    <value2> : <code to be executed>
    etc...
ENDCASE
```

E.g:

```
CASE OF num1
    1 : OUTPUT "num1 is 1"
    2 : OUTPUT "num1 is 2"
    3 : OUTPUT "num1 is 3"
ENDCASE
```

An OTHERWISE clause can be added, which acts similarly to an ELSE clause. It must always be the last case.

```
CASE OF <variable>
    <value1> : <code to be executed>
    <value2> : <code to be executed>
    etc...
    OTHERWISE : <code to be executed>
ENDCASE
```

E.g:

```
CASE OF num1
    1 : OUTPUT "num1 is 1"
    2 : OUTPUT "num1 is 2"
    3 : OUTPUT "num1 is 3"
    OTHERWISE : OUTPUT "num1 is not 1, 2 or 3"
ENDCASE
```
