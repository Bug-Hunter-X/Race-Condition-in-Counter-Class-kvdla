# Race Condition in Counter Class

This repository demonstrates a race condition in a simple counter class.  The `Counter` class is intended to increment a counter variable. However, when used in a multithreaded environment without proper synchronization, the final count might be less than the expected value due to race conditions.

The `Counter.java` file contains the buggy code;  `CounterSolution.java` provides a solution using the `synchronized` keyword to ensure atomicity.

## How to Reproduce
1. Compile and run `Counter.java`. 
2. Observe that the final count is often less than 20000, indicating a race condition.
3. Compile and run `CounterSolution.java` to see the correct, synchronized version.

## Learning Points
This example highlights the importance of synchronization in concurrent programming to avoid race conditions and ensure data integrity.