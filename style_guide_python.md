# Code and Documentation Style Guide

## Introduction

This document serves as a style guide and template for writing code and generating documentation for personal projects. It ensures that the codebase is maintainable, readable, and facilitates automated documentation generation.

## Code Structure

### Header Comments

- Every file must have a header with the following information:
  - Title: The name of the script.
  - Description: A brief summary of what the script does.
  - Author: The name of the developer.
  - Date Created: When the script was initially created (format: YYYY-MM-DD).
  - Version: The current version of the script.

Example:

```python
"""
Title: Data Processor
Description: This script processes data from CSV files and generates reports.
Author: [Your Name]
Date Created: 2023-11-05
Version: 1.0.0
"""
```

### Class and Function Documentation

- Each class and function should have a docstring that includes:
  - A description of its functionality.
  - Parameters with data types and what they represent.
  - Return values with data types and what they represent.
  - Exceptions that the function might raise.

Example:

```python
def calculate_statistics(data):
    """
    Calculates and returns statistical data.

    Parameters:
    - data (list of int): The list of numbers to calculate statistics on.

    Returns:
    - stats (dict): Dictionary containing mean, median, and mode.

    Raises:
    - ValueError: If the input data is not a list of numbers.
    """
    # Function body...
```

### Inline Comments

- Use inline comments to explain complex or non-obvious code constructs.

Example:

```python
x += 1  # Compensate for the index starting at 0
```

## Logical Tags for Documentation

- Specific tags should be used for automated documentation extraction:
  - `@description`: Describes what the function or class does.
  - `@param`: Details about the parameters.
  - `@return`: Information about the return values.
  - `@raise`: Exceptions that may be raised.

## Markdown Document Generation

- A Python script should read these tags to generate a documentation file in Markdown format.

## Template for New Code

- Use the provided file template that includes header comments and placeholders for necessary documentation.

## Code Formatting: Following PEP 8 Guidelines

- PEP 8 is the style guide for Python code. Adhering to PEP 8 means:
  - Indentation should be 4 spaces per level, not tabs.
  - Lines should be 79 characters long or less.
  - Use blank lines to separate functions and classes, and larger blocks of code inside functions.
  - When possible, put comments on a line of their own.
  - Use docstrings.
  - Use spaces around operators and after commas, but not directly inside bracketing constructs.
  - Name your classes and functions consistently; the convention is to use `CamelCase` for classes and `snake_case` for functions and variables.
  - Don't use fancy encodings if your code is meant to be used in international environments. Plain ASCII works best in any case.

For a full guide on PEP 8, refer to the [PEP 8 documentation](https://www.python.org/dev/peps/pep-0008/).

## Revision History

- Keep track of significant changes to the document here.

| Version | Date       | Author       | Changes Made                       |
|---------|------------|--------------|------------------------------------|
| 0.0.1   | 2023-11-05 | [Your Name] | Initial creation of the style guide. |
