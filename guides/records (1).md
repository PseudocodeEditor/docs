---
description: Introduction to Records
---

# Records

A record is a composite data type that contains multiple different data types. It contains multiple data items that can be accessed via dot notation. They are defined with keywords TYPE, ENDTYPE, and contain declarations:

```
TYPE <data type name>
    DECLARE <item1> : <type>
    DECLARE <item2> : <type>
    ...
ENDTYPE
```

Then, variables can be declared of the data type that has been defined, to be able to access elements within. To access items within the data type, the name of the variable is used, followed by a dot, then the name of the item to be accessed.

```
TYPE Person
    DECLARE FirstName : STRING
    DECLARE LastName : STRING
    DECLARE FavFood : STRING
    DECLARE Age : INTEGER
ENDTYPE

DECLARE Friend1 : Person

Friend1.FirstName <- "Jack"
Friend1.LastName <- "Pollier"
Friend1.FavFood <- "Lasagna"
Friend1.Age <- 17
```
