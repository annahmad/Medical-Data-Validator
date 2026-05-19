# Medical Records Validator

A Python workshop project that validates a list of medical records against a set of formatting and type constraints using regex and custom rules. Built as part of the [freeCodeCamp Python Certification]((https://www.freecodecamp.org/learn/python-v9)).
 

## What It Does

- Checks that the input data is a list or tuple
- Validates each record is a dictionary with the correct keys
- Enforces formatting rules on each field using regex and type checks
- Prints a specific error message for every invalid field found
- Returns `True` if all records are valid, `False` otherwise

## Fields Validated

| Field | Rule |
|---|---|
| `patient_id` | String matching pattern `P` + digits (case-insensitive) |
| `age` | Integer, must be 18 or older |
| `gender` | String, must be `male` or `female` (case-insensitive) |
| `diagnosis` | String or `None` |
| `medications` | List of strings |
| `last_visit_id` | String matching pattern `V` + digits (case-insensitive) |

## Example Output
Unexpected format 'patient_id: p1002' at position 1.
Unexpected format 'gender: male' at position 1.
Unexpected format 'last_visit_id: v2302' at position 1.

## How to Run

```bash
python medical_validator.py
```

## Technologies Used

- Python 3
- `re` module (regular expressions)

## Author
Ann Ahmad
