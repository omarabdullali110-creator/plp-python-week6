## Files
 `safe_tools.py` - three functions (`safe_divide`, `safe_number`, `get_field`) that use try/except so they return a friendly message instead of crashing.
 `README.md` - this file: the assignment title, a description of each file, and the answer below.

## Why can an `if` check not catch "abc" on its own?
An `if` check can only test for a problem you already thought of, such as `if b == 0`. The text "abc" is a different kind of bad input: it only fails when `int()` actually tries to convert it and raises a `ValueError`. Writing an `if` for every possible bad value is impractical, whereas `try / except ValueError` catches the failure at the moment it happens and keeps the program running.