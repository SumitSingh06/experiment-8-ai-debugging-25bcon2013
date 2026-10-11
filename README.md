# Experiment 8: Fixing a Buggy Python Script Using AI

## Objective
To identify and fix Python programming errors using AI-assisted debugging and unit testing.

## Bugs Identified
1. **Average calculation:** Incorrect denominator caused wrong results and division by zero.
2. **Passing boundary:** The condition `>` incorrectly treated 40 as a failing mark.
3. **Grade ordering:** The Distinction condition was checked after lower grade conditions.

## Fixes Applied
- Changed the average denominator to `len(marks)`.
- Changed the passing condition to `mark >= PASS_MARK`.
- Checked the Distinction condition before the other grade conditions.

## Testing
The corrected program was tested using Python's `unittest` framework.

Command:
```bash
python test_student_utils.py
```

Expected result: All 9 tests pass.

## RED → FIX → GREEN
- **RED:** Tests failed on the buggy implementation.
- **FIX:** Corrected the identified errors.
- **GREEN:** Reran the same tests successfully.

## Limitation
The program does not handle an empty list of marks.
