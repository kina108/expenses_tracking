# Expense Tracker (Streamlit)

A web-based expense tracking application built with **Streamlit** and **SQLite**.  
The app allows users to record daily expenses, manage existing entries, and view monthly spending summaries with visualizations.

This application is deployed on **Streamlit Community Cloud** at https://expensestracking.streamlit.app/.

---

## Overview

The Expense Tracker provides a simple interface for:
- Recording expenses
- Editing and deleting existing entries
- Reviewing monthly spending by category
- Visualizing spending trends over time

All data is stored locally in a SQLite database created at runtime.

---

## How to Use the App

### 1. Add an Expense
- Navigate to the **“Add an expense”** section
- Select a date (defaults to today)
- Enter a category (required)
- Enter an amount (must be ≥ 0)
- Click **Add**

The expense is saved and the app refreshes automatically.

---

### 2. View All Expenses
- Scroll to **“All expenses (edit / delete)”**
- All recorded expenses are displayed in a table
- Each expense has a unique **ID**

---

### 3. Edit an Expense
- Use the **Select expense ID** dropdown to choose an entry
- The current values are prefilled in the **Update selected expense** form
- Modify the date, category, or amount
- Click **Update**

Changes are saved immediately.

---

### 4. Delete an Expense
- Select an expense ID
- Click **Delete**
- The selected expense is permanently removed

---

### 5. View Monthly Summary
- Go to the **“Monthly summary”** section
- Enter a month in the format:YYYY-MM


- The app displays:
- Category totals table
- Total amount spent
- Pie chart showing category distribution
- Daily spending line chart (if data exists)

---

## Visualizations

- **Category Table**: Summarized spending per category
- **Total Metric**: Total spending for the selected month
- **Pie Chart**: Category share of total spending
- **Line Chart**: Daily spending trend over the month

If no data exists for the selected month, an informational message is shown instead.

---

## Data Storage

- Data is stored in a local SQLite database (`expenses.db`)
- Dates are stored in ISO format (`YYYY-MM-DD`)
- Monthly filtering is performed using string-based matching

### Streamlit Community Cloud Note
On Streamlit Community Cloud:
- The database file is stored on the app’s ephemeral filesystem
- Data may reset if the app is redeployed or restarted

---

## Technology Stack

- **Streamlit** – UI framework
- **SQLite** – Local database
- **Pandas** – Data handling
- **Matplotlib** – Charts and visualizations
- **Python 3**

---

