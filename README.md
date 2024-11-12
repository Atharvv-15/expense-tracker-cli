# Expense Tracker CLI

[roadmap.sh Expense Tracker Project](https://roadmap.sh/projects/expense-tracker).

A simple command-line interface tool to track your daily expenses. Built with Python, this application allows you to add, update, delete, and view your expenses with ease.

## Features

- Add new expenses with descriptions and amounts
- Update existing expenses
- Delete expenses
- View monthly summaries
- List all expenses
- Colored output for better readability

## Prerequisites

- Python 3.x
- pip (Python package installer)

## Installation

1. Clone this repository:

bash
git clone <repository-url>
cd expense-tracker-cli

2. Install required packages:

bash
pip install colorama


## Usage

### Adding an Expense
bash
python expense-tracker.py add "description" amount
Example:
python expense-tracker.py add "Groceries" 50.50


### Updating an Expense
bash
Update description
python expense-tracker.py update id "new description"
Update amount
python expense-tracker.py update id amount
Update both
python expense-tracker.py update id "new description" amount


### Viewing Summary
bash
View total expenses
python expense-tracker.py summary
View expenses for a specific month (1-12)
python expense-tracker.py summary 3 # Shows March expenses


### Listing All Expenses

## Data Storage

Expenses are stored in a CSV file (`expense.csv`) with the following structure:
- id: Unique identifier for each expense
- date: Date of the expense
- description: Description of the expense
- amount: Amount spent

## Error Handling

The application includes error handling for:
- Invalid amounts
- Empty descriptions
- Invalid IDs
- File not found scenarios
- Invalid month numbers
- Invalid data formats

## Color Coding

- Green: Success messages
- Red: Error messages
- Yellow: Amount values
- Cyan: Headers in list view

