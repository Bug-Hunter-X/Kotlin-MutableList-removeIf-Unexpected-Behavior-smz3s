# Kotlin MutableList removeIf Unexpected Behavior

This repository demonstrates an uncommon bug in Kotlin related to the `removeIf` function when used with a mutable list.  The `removeIf` function iterates through the list and removes elements based on a given predicate. However, if the predicate's execution modifies the list (e.g., adding or removing elements), the iteration process can be disrupted, leading to unexpected results or exceptions.

The `bug.kt` file demonstrates this issue, while `bugSolution.kt` shows a correct approach.

## Bug Reproduction

1. Clone this repository.
2. Compile and run `bug.kt`. 
3. Observe that the output is not as expected.

## Solution

The `bugSolution.kt` file demonstrates a solution using an iterator to safely modify the list during iteration.