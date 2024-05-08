# Java Sample Calculator

Implementing arithmetic operator buttons in the calculator program involves handling several subtleties. Firstly, the program needs to remember the last value entered and the operator used. Additionally, it needs to keep track of whether a value is being entered or if it's in the middle of a calculation. The value currently being built up can be obtained from the display field.

When an operator button is clicked and two operands are available, the display is updated with the result of the saved operation. The first digit button clicked after an operator clears the display, while subsequent digit buttons append to the display. The "=" button puts the calculator into the same state as it was at the beginning, clearing the saved operation.

For example, consider the input "3 + 4 =" followed by "5 * 6". When the "=" button is clicked, the last operator ("+") is executed, and "=" becomes the last operator. When the "*" button is clicked, the calculate method receives the last value (7), the display value (5), and the last operator ("="). It should simply return the second operand (5), which will later be combined with the "*" operator.

By understanding and implementing these behaviors, the calculator can accurately perform arithmetic operations while providing a user-friendly interface. Our aim was to design a calculator program that incorporates these features.
