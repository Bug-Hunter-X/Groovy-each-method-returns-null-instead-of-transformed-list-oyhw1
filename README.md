# Groovy each() Method Unexpected Null Return

This example demonstrates a common pitfall in Groovy: the `each()` method doesn't return a modified list.  Many developers expect it to behave like `map()`, but it's primarily designed for side effects (like printing).  This repo contains the erroneous code and its corrected version.

## Bug
The `bug.groovy` file shows the incorrect use of `each()` to transform a list.  It produces a `null` output instead of the transformed list.

## Solution
The `bugSolution.groovy` file provides the correct way to transform a list using the `collect()` method, which produces the expected result.