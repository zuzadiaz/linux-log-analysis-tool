# Log Data Analysis with Python

## Overview

This project is a Python-based log analysis tool built in Ubuntu Linux (WSL).

The script processes Linux authentication logs, extracts structured data using regular expressions (regex), analyzes failed login activity, identifies recurring patterns, and summarizes repeated events.

## Technologies Used

- Python
- Ubuntu Linux (WSL)
- Regex
- Log Data Analysis
- Command-line interface (CLI)

## Features

- Reads and processes Linux authentication logs
- Extracts IP addresses from log records
- Identifies failed login activity
- Counts repeated events
- Summarizes recurring patterns in log data

## How to Run

Run the script in Linux terminal:

```bash
python3 log_monitor.py
```


## Detection Logic

- LOW severity: 1–2 failed login attempts
- MEDIUM severity: 3–4 failed login attempts
- HIGH severity: 5+ failed login attempts

The script flags repeated failed SSH login attempts as potentially suspicious activity.


## Sample Output

```text
=== SSH Failed Login Analysis ===

IP Address: 192.168.1.45
Failed Attempts: 1
Severity Level: LOW

IP Address: 203.0.113.10
Failed Attempts: 3
Severity Level: MEDIUM
ALERT: 203.0.113.10 may be suspicious.
```

## Skills Demonstrated

- Python
- Data Analysis
- Log Analysis
- Data Processing
- Regular Expressions (Regex)
- Linux
- File Handling
- Automation
- Problem Solving

