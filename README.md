# Playwright Test Automation Project

This repository contains a Python Playwright automation script for validating the Pixels Suite Chat Translator using test cases stored in the Excel workbook.

## Project Files

- `IT23276314_test_automation.py` - Playwright automation script.
- `IT23276314_Assignment 1 - Test cases.xlsx` - Test case workbook used as the default input file.
- `IT23276314_requirements.txt` - Python package dependencies.
- `IT23276314_git_repository_link.txt` - Public Git repository URL for submission.

## Prerequisites

- Python 3.10 or newer.
- Git.
- Internet access, because the test opens `https://www.pixelssuite.com/chat-translator`.

## Install Dependencies

Create and activate a virtual environment:

```bash
python -m venv .venv
```

On Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

On macOS/Linux:

```bash
source .venv/bin/activate
```

Install Python packages:

```bash
pip install -r IT23276314_requirements.txt
```

Install the Playwright browser binaries:

```bash
python -m playwright install
```

## Run the Tests

Run with the browser visible:

```bash
python IT23276314_test_automation.py
```

Run in headless mode:

```bash
python IT23276314_test_automation.py --headless
```

The script reads `IT23276314_Assignment 1 - Test cases.xlsx`, enters each Singlish input into the translator, compares the Sinhala output when an expected value is available, and writes the actual output and status back into the workbook.

## Useful Options

Use a different Excel file:

```bash
python IT23276314_test_automation.py --excel "path/to/test-cases.xlsx"
```

Save results to a separate workbook:

```bash
python IT23276314_test_automation.py --output "results.xlsx"
```

Use a different frontend URL:

```bash
python IT23276314_test_automation.py --url "https://example.com"
```

## Git Submission

Make sure this project is pushed to a public Git repository before submission. Add the public repository URL to `IT23276314_git_repository_link.txt`.
