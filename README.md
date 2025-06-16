# python-capstone-finance-tracker

Simple command-line personal finance tracker that allows users to **log expenses**, **categorize them**, and **view summaries** of their expenses.

## Features
- Add expenses with a description, category, and amount.
- View all recorded expenses, organized by category.
- View a summary of total spending per category.
- Input validation and basic error handling to ensure clean data entry.

## Run the Script
1. Save the script as `finance_tracker.py`
2. Run it using:
```bash
python finance_tracker.py
```

## Functions

`add_expense()`: Prompts the user to enter an expense description, category, and amount. Performs input validation (non-empty strings and valid float values). Stores each expense as a `(description, amount)` tuple under its category in a global dictionary.

`view_expenses(data)`: Displays all stored expenses grouped by category. Each entry is printed with its description and dollar amount.

`view_summary(data)`: Calculates and displays the **total amount spent** in each category.

`main`: Displays an interactive menu. Accepts user choices and routes to the appropriate function (`add_expense`, `view_expenses`, or `view_summary`), while handling invalid input and exits on command.

## Python Concepts used
- **Functions**: Used to organize code for each operation
- **Dictionaries**: Used to store expenses grouped by category
- **Tuples**: Each expense is stored as a `(description, amount)` tuple
- **Loops**: 
  - `while` loops for repeated prompts and menu navigation
  - `for` loops for iterating over categories and expenses
- **Conditionals**: `if` statements for checking input and managing flow
- **Exception Handling**: `try/except` blocks to handle:
  - Invalid numerical inputs
  - Empty inputs
  - Unexpected runtime errors
- **String Methods**: `.strip()` to clean user input and make sure no empty input is accepted
  
