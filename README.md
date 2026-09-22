# 🎫 Customer Support Ticket Analyser

## 📌 Project Overview

The **Customer Support Ticket Analyser** is a Python-based project designed to store, clean, and analyse customer support tickets.

The project processes customer ticket information such as **ticket number, customer name, issue description, and priority**. It also allows users to add new tickets and generates useful insights from the available ticket data.

This project was developed as part of a **Python Module End Assignment** to practise Python data structures, loops, functions, conditional statements, string operations, and sets.

---

## 🎯 Project Objectives

The main objectives of this project are:

* Store customer support tickets using a dictionary of lists.
* Add new tickets dynamically using user input.
* Automatically generate ticket numbers.
* Validate ticket priorities.
* Clean and standardise issue descriptions.
* Search tickets using specific keywords.
* Analyse ticket priority levels.
* Identify the ticket with the longest issue description.
* Extract and sort unique words from ticket descriptions.

---

## 🛠️ Technologies Used

* **Python**
* **Google Colab**
* Python Lists
* Python Dictionaries
* Python Sets
* Functions
* Loops
* Conditional Statements
* String Operations

---

## 📊 Dataset

The project starts with **10 preloaded customer support tickets**.

Each ticket contains:

| Column            | Description              |
| ----------------- | ------------------------ |
| Ticket_No         | Unique ticket number     |
| Customer_Name     | Name of the customer     |
| Issue_Description | Customer's support issue |
| Priority          | High, Medium, or Low     |

New tickets can also be added by the user during program execution.

---

## 🔄 Project Workflow

```text
Initial Ticket Data
        ↓
Display Tickets
        ↓
Add New Tickets
        ↓
Validate Priority
        ↓
Clean Issue Descriptions
        ↓
Keyword Analysis
        ↓
Priority Analysis
        ↓
Longest Issue Analysis
        ↓
Unique Word Extraction
        ↓
Final Summary & Insights
```

---

## 🧹 Data Cleaning

The issue descriptions are cleaned using Python string operations.

The cleaning process includes:

* Converting text to lowercase
* Removing punctuation such as `. , ! ? -`
* Removing leading and trailing spaces
* Converting multiple spaces into a single space
* Replacing shorthand/slang such as `ok` with `okay`

### Example

**Before cleaning:**

```text
" GREAT support! issue resolved. "
```

**After cleaning:**

```text
"great support issue resolved"
```

---

## 🔍 Keyword Analysis

A reusable Python function is created to count the number of tickets containing specific keywords.

The project analyses the following words:

* `poor`
* `good`
* `slow`
* `excellent`

Example:

```python
def count_tickets_with_word(word):
    count = 0

    for issue in ticket_data['Issue_Description']:
        words = issue.split()

        if word.lower() in words:
            count += 1

    return count
```

---

## 📈 Priority Analysis

The project calculates the number of tickets for each priority level:

* 🔴 High
* 🟡 Medium
* 🟢 Low

This helps understand the distribution of customer support workload.

---

## 📝 Longest Issue Description

The program calculates the word count of each cleaned issue description and identifies the ticket with the longest description.

The analysis displays:

* Ticket Number
* Customer Name
* Cleaned Issue Description
* Word Count

---

## 🔤 Unique Word Analysis

A Python `set` is used to identify unique words across all ticket descriptions.

The project displays:

* Total number of unique words
* Alphabetically sorted list of unique words

Using a set automatically removes duplicate words.

---

## 💡 Key Findings

The analysis provides insights into:

1. Total number of customer support tickets.
2. Distribution of High, Medium, and Low priority tickets.
3. Frequency of common keywords such as `poor`, `good`, `slow`, and `excellent`.
4. Ticket containing the longest issue description.
5. Total number of unique words used in customer issues.

The exact findings depend on the additional tickets entered by the user during program execution.

---

## 📌 Sample Output

```text
CUSTOMER SUPPORT TICKET ANALYSER - FINAL SUMMARY

Total Tickets: 10

High Priority: 4
Medium Priority: 3
Low Priority: 3

Tickets containing 'poor': 2
Tickets containing 'good': 2
Tickets containing 'slow': 2
Tickets containing 'excellent': 1

Longest Issue Word Count: 6

Total Unique Words: ...
```

> **Note:** The output values may change when additional tickets are added.

---

## 📚 Python Concepts Practised

This project helped practise the following Python concepts:

* Variables
* Lists
* Dictionaries
* Sets
* `input()`
* `print()`
* `if-else`
* `while` loop
* `for` loop
* Functions
* `append()`
* `replace()`
* `split()`
* `strip()`
* `lower()`
* `join()`
* `count()`
* `len()`
* `sorted()`

---

## 🚀 Future Improvements

The project can be further enhanced by adding:

* Sentiment analysis
* Issue category classification
* Customer satisfaction analysis
* Ticket status tracking
* Response-time analysis
* Data visualisation using Matplotlib
* Interactive dashboards using Power BI
* CSV/Excel file import and export
* Automated ticket reports

---

## 👨‍💻 Author

**Kesavaraj M**

Aspiring Data Analyst | Python | SQL | Excel | Power BI

📍 Erode, Tamil Nadu, India

---

## ⭐ Conclusion

The **Customer Support Ticket Analyser** demonstrates how Python can be used to manage and analyse customer support data.

The project combines **data structures, text cleaning, functions, loops, conditional statements, and basic analytical techniques** to convert raw customer ticket information into meaningful insights.

