---
description: Introduction to Loop Structures
---

# Loop Structures

There are 3 types of loop structures that are used within pseudocode, which are pre-condition, post-condition and count controlled loops.

### Pre-Condition (WHILE)

This type of loop is likely the one that most are familiar with, where the loop is controlled by a condition set before the loop. It follows the structure of WHILE, ENDWHILE.

```
WHILE <condition>
    <code to be executed>
ENDWHILE
```

It may not execute at all, depending on the set condition. E.g:

```
WHILE num1 < 5
    num1 <- num1 + 1
ENDWHILE
```

The expression will continue evaluating until the condition becomes FALSE, at which point the loop terminates.

### Post-Condition (REPEAT)

This type of loop depends on a condition set after the code within it has executed once, as the condition is evaluated after the code. It follows the structure of REPEAT, UNTIL.

```
REPEAT 
    <code to be executed>
UNTIL <condition>
```

E.g:

```
REPEAT
    num1 <- num1 + 1
UNTIL num1 = 10
```

### Count-Controlled (FOR)

This type of loop depends on a counter set within its initial statement. It follows the structure of FOR, TO, NEXT.

```
FOR <integer variable> TO <desired limit>
    <code to be executed>
NEXT <integer variable that was used>
```

The value of the variable used as a counter can be assigned within the FOR statement.&#x20;

```
FOR x <- 1 TO 10
    OUTPUT x
NEXT x
```

The default increment value for the count variable is 1, however this can be changed with the addition of an extra keyword, STEP. A negative increment can be used, and as soon as the variable reaches a value equal to or above the limit, the loop terminates.

```
FOR <variable> TO <limit> STEP <increment>
    <code to be executed>
NEXT <variable>
```
