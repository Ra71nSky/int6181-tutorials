# INT6181 Tutorials 6 & 7

Unit tests written for Tutorial 6 (test-first practice), and the GitHub Actions workflow
for Tutorial 7.

## tutorial_6 — Test Code in Scale & Fix with Debugger

Three modules, three hand-written `unittest` suites:

| module | test file | what it covers |
|---|---|---|
| `password_validator.py` | `test_password_validator.py` | type, length 8-20, no whitespace, four character classes |
| `triangle.py` | `test_triangle.py` | numeric/non-bool sides, > 0, triangle inequality, type, area to 4 dp |
| `parking_fee.py` | `test_parking_fee.py` | positive hours, first hour free, ceil per hour, 24h cap, multi-day |

Run them:

```bash
cd tutorial_6
python -m unittest discover -v
```

## tutorial_7 — Automate Tests with GitHub Actions

The workflow lives in `.github/workflows/python-tests.yml` and runs the provided test
suite on every push and pull request, across Python 3.10 / 3.11 / 3.12.
