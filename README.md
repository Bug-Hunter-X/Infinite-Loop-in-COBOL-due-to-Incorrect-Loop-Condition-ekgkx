# COBOL Infinite Loop Bug

This repository demonstrates a common error in COBOL programs: an infinite loop caused by an incorrect loop condition.  The code attempts to sum numbers from 1 to 100, but due to a flawed condition in the `PERFORM VARYING` statement, the loop continues indefinitely. 

**Bug:** The `PERFORM VARYING` statement doesn't increment `WS-COUNTER`.  

**Solution:** The loop condition is corrected to increment `WS-COUNTER`.  The corrected code is provided in `bugSolution.cob`.

This example highlights the importance of carefully reviewing loop conditions to prevent infinite loops and resource exhaustion in COBOL programs.