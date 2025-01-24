# Kotlin map() Function: Handling Null and Empty Lists

This repository demonstrates the behavior of Kotlin's `map()` function when dealing with null and empty lists.  It highlights a common pitfall where developers might not anticipate the function's response to these edge cases.

## The Problem

The `map()` function, when applied to a null list, will return null.  When applied to an empty list, it will return an empty list.  Failure to handle these conditions correctly can lead to null pointer exceptions or unexpected outputs.

## The Solution

The best approach is to always check for null values using the safe call operator (`?.`) and the Elvis operator (`?:`) to provide a default value.  This ensures that the code handles null inputs gracefully without crashing.

## Files:

* `BuggyMap.kt`: Shows the code exhibiting the potential problem with null values.
* `FixedMap.kt`: Demonstrates the corrected code that safely handles null and empty lists.