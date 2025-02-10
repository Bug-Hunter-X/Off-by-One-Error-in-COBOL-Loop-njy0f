# Off-by-One Error in COBOL Loop

This repository demonstrates a common off-by-one error in COBOL programming.  The provided COBOL program attempts to count from 1 to 10 but incorrectly uses a loop condition that results in an off-by-one error. The solution demonstrates the correct way to implement the loop to achieve the intended count.

## Bug Description
The `PERFORM VARYING` statement, while powerful, is prone to off-by-one errors if the loop termination condition isn't carefully constructed. In this case, the loop continues as long as `I` is greater than 10. This means the loop iterates one time too many, resulting in an incorrect final count.