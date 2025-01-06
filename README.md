# Unexpected Implicit Return in PHP if Statements

This example demonstrates a common, yet subtle, error in PHP: implicit returns within `if` statements.  When a `return` statement is used inside an `if` block, and no explicit `return` is present outside it, PHP will implicitly return if the `if` condition evaluates to true. This can lead to unexpected behavior, especially in larger functions or when expecting code execution after the `if` block regardless of the condition.

The `bug.php` file shows the erroneous code, while `bugSolution.php` presents the corrected version.

## How to Reproduce

1.  Run `bug.php`.
2. Observe the unexpected output compared to what might be initially expected. 
3. Run `bugSolution.php` to see the corrected behavior.