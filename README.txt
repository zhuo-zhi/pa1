1. Give three examples of Python programs that use binary operators and/or builtins from this PA, but have different behavior than your compiler. For each, write:
- a sentence about why that is
- a sentence about what you might do to extend the compiler to support it

1) In this PA, Print() cannot support multiple arguments while Python can, e.g. print(1, 2, 3). To support this feature, we have to enable parsing multiple arguments in the ArgList for print() and extend the corresponding imports function to accept multiple arguments.

2) In this PA, print() returns a 32-bit integer, e.g. abs(print(-1)) while print() returns None in Python. To support this feature, we have to let the corresponding imports function return nothing.

3) In this PA, max()/min() doesn't support multiple arguments while Python can, e.g. max(1, 2, 3). To support this feature, we have to enable parsing multiple arguments in the ArgList for max()/min() and modify the comparing logic in the corresponding imports functions.

2. What resources did you find most helpful in completing the assignment?

1) https://webassembly.org/specs/

2) https://lezer.codemirror.net/docs/ref/#common.TreeCursor

3. Who (if anyone) in the class did you work with on the assignment? (See collaboration below)

In this assignment, I do not collaborate with other students. Piazza and TA video is very helpful.