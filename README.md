# Go Array Index Out of Bounds
This repository demonstrates a common error in Go: an array index out of bounds error.  The `bug.go` file contains code that attempts to access an element beyond the array's bounds, leading to a runtime panic. The solution is provided in `bugSolution.go`. 

The bug arises because Go arrays are zero-indexed, and their valid indices range from 0 to the array's length minus 1. Accessing an element using an index equal to or greater than the length will cause a panic.

This example highlights the importance of careful array index handling in Go to avoid runtime errors.  Always ensure that your indices are within the valid range before accessing array elements.  Using the `len()` function is frequently helpful for determining the valid upper bound of an array index.