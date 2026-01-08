#  Habit Tracker - Python Portfolio Project

A comprehensive habit tracking application combining **Object-Oriented Programming (OOP)** with **Functional Programming (FP)**.

##  Features

- ✅ **OOP Design**: Habit class with proper encapsulation
- ✅ **FP Analytics**: Pure functions for data analysis
- ✅ **SQLite Database**: Persistent data storage
- ✅ **CLI Interface**: User-friendly command line
- ✅ **Unit Tests**: 85%+ test coverage
- ✅ **4 Weeks Data**: Predefined test habits

##  Installation

```bash
git clone https://github.com/khouloudchebboubi22-ui/oofpp-habit-tracker.git
cd oofpp-habit-tracker
pip install -r requirements.txt
Usage Examples
bash
# Create a new habit
python run.py create --name "Morning Exercise" --periodicity daily

# Complete a habit
python run.py complete --name "Morning Exercise"

# List all habits
python run.py list

# Show analytics
python run.py analytics

# Generate test data (4 weeks)
python run.py generate-test-data
 Running Tests
bash
# Run all tests
pytest

# Run with coverage report
pytest --cov=src --cov-report=html
Analytics Functions
The analytics module implements functional programming:

filter_by_periodicity() - Filter habits by daily/weekly

get_longest_streak_all() - Longest streak across all habits

get_longest_streak_for_habit() - Streak for specific habit

get_daily_habits() - All daily habits

get_weekly_habits() - All weekly habits

 Project Structure
text
oofpp-habit-tracker/
├── src/                    # Source code
│   ├── habit.py           # OOP: Habit class
│   ├── storage.py         # SQLite database
│   ├── analytics.py       # FP: Analytics functions
│   └── cli.py            # CLI interface
├── tests/                 # Test suite
├── data/                  # Test data
├── requirements.txt       # Dependencies
├── run.py                # Main entry point
└── README.md             # Documentation
 Author
Khouloud Chebboubi
Matriculation: 102303255
Course: Object-Oriented and Functional Programming with Python (DLBDSOOFPP01)
IU International University of Applied Sciences

 GitHub Repository
https://github.com/khouloudchebboubi22-ui/oofpp-habit-tracker

text

---

## ** File 4: `run.py`**
```python
#!/usr/bin/env python3
"""
Main entry point for Habit Tracker.
Run: python run.py --help
"""

from src.cli import cli

if __name__ == "__main__":
    cli()
