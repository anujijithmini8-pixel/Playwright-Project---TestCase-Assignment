# Playwright Test Automation (IT23145702)

This repository runs a Python + Playwright script that reads test cases from an Excel sheet, executes them against the target web UI, and writes back **Actual output** and **Status** into the same workbook.

## Prerequisites

- Python 3.10+ (the script uses `str | None` type syntax)
- Internet access (the script opens the target URL in a real browser)

## Install Dependencies

```powershell
python -m pip install -r requirements.txt
python -m playwright install chromium
```

## Run The Automation

The default Excel file is:

- `IT23145702_Assignment 1 - Test cases.xlsx` (fallback: `Assignment 1 - Test cases.xlsx`)

Run:

```powershell
python .\IT23145702_test_automation.py
```

Optional arguments:

```powershell
python .\IT23145702_test_automation.py --excel ".\IT23145702_Assignment 1 - Test cases.xlsx" --headless
```

Environment variables:

- `FRONTEND_URL` (overrides the default URL)

