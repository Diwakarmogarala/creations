# Python Calculator

A simple command-line calculator built with Python. It supports addition, subtraction, multiplication, and division.

## Features

- Performs calculations with whole numbers and decimals.
- Checks for division by zero.
- Displays the menu again when an option of 5 or higher is entered.
- Allows repeated calculations until the user types `bye`.

## Requirements

- Python 3
- No external libraries required.

## How to Run

1. Save the code in a file, such as `calculator.py`.
2. Make sure the file calls the calculator function at the end:

   ```python
   calci()
   ```

3. Open a terminal in the folder containing the file and run:

   ```bash
   python calculator.py
   ```

## How to Use

1. Select an operation:
   - `1` — Addition
   - `2` — Subtraction
   - `3` — Multiplication
   - `4` — Division
2. Enter the first and second numbers.
3. View the result.
4. Type `yes` to perform another calculation or `bye` to exit.

Entering `5` or higher restarts the menu without asking for numbers.

## Example

```text
Type : 1 for add,
       2 for subtract,
       3 for multiply and
       4 for divide
 Select option : 1
Enter first value : 10
Enter Second value : 5
 10.0 + 5.0  =  15.0
If you want to continue type : yes
If you want to exit type : bye
Type your response : bye
```

## Functions

| Function | Description |
|---|---|
| `add(a, b)` | Returns the sum of two numbers. |
| `subtract(a, b)` | Subtracts the second number from the first. |
| `multiply(a, b)` | Returns the product of two numbers. |
| `divide(a, b)` | Returns the quotient, or `"This was not possible"` when the second number is zero. |
| `calci()` | Displays the menu, reads input, and controls repeated calculations. |

## How the Loop Works

The calculator uses `while True` to repeat.

- `continue` skips the rest of the current iteration and returns to the menu when the selected option is `5` or higher.
- `break` exits the loop when the user types `bye`.

## Current Limitations

- Non-numeric input for the operation or numbers causes a `ValueError`.
- Zero and negative operation choices are not rejected; they prompt for numbers but produce no calculation.
- Responses must be exactly `yes` or `bye`. Other responses cause the loop to run without displaying another prompt.
