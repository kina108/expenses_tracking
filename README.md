# Expense Tracker (Streamlit)

A web-based expense tracking application built with **Streamlit** and **SQLite**.  
The app allows users to record daily expenses, manage existing entries, and view monthly spending summaries with visualizations.

This application is deployed on **Streamlit Community Cloud**.

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
- Enter a month in the format:

