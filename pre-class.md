# **Pre-Class Self-Study: Introduction to Data Analysis with Pandas**

⏱️ Estimated Time: 45-60 minutes

📅 Complete Before: Class Session 1

## **🎯 What You'll Learn Before Class**

By completing this pre-class work, you will:

* **Understand** the difference between a Series and a DataFrame.  
* **Identify** how Python represents missing data.  
* **Recognize** the basic structure of the Pandas library.

## **💻 Part 1: Environment Setup (15-20 min)**

### **Prerequisites**

Ensure you have Python installed (Anaconda distribution recommended).

### **Installation Instructions**

Step 1: Install Required Libraries

Open your terminal or command prompt and run:

```
pip install pandas numpy matplotlib sqlalchemy
```

Step 2: Verify Installation

Open a Jupyter Notebook and run this cell:

```
import pandas as pd
import numpy as np
import sqlite3

print(f"Pandas version: {pd.__version__}")
print(f"NumPy version: {np.__version__}")
print("✅ Ready for class!")
```

Step 3: Organize Your Data

Create a folder named data in your project directory and move the following files into it:

* ex1.csv through ex5.csv  
* Resaleflatpricesbasedonregistrationdate.xlsx \- 2017.csv  
* unit-1-4.db

## **📚 Part 2: Course Introduction (10-15 min)**

### **What is Exploratory Data Analysis (EDA)?**

EDA is "detective work" for data. Before we build machine learning models or fancy dashboards, we must understand what we are looking at.

Real-World Example:

Imagine you are a real estate agent. You have a spreadsheet of 10,000 home sales.

* **EDA** is figuring out: "Are there any homes sold for $0 (errors)?" or "What is the average price in Yishun?"  
* **Data Cleaning** is fixing the row that says "3 Room Flat" where the price is missing.

### **Why This Matters**

Data in the real world is **never** clean. 80% of a Data Scientist's job is cleaning and arranging data. This lesson gives you the tools to do that 80% efficiently.

## **🧠 Part 3: Basic Concepts (20-25 min)**

### **Concept 1: The DataFrame**

Think of a **DataFrame** like a programmable Excel sheet.

* It has **rows** (observations) and **columns** (variables).  
* Unlike Excel, we manipulate it with code, making our work reproducible.

**Try It Yourself:**

```
import pandas as pd
data = {'Town': ['Bedok', 'Tampines', 'Yishun'],
        'Price': [450000, 500000, 380000]}
df = pd.DataFrame(data)
print(df)
```

### **Concept 2: Missing Data (NaN)**

Real data has holes. In Python/Pandas, a missing number is often represented as NaN (Not a Number).

* You cannot do math with NaNs (mostly). 5 \+ NaN \= NaN.  
* We have to decide: do we fill the hole, or throw away the row?

## **✅ Pre-Class Self-Check**

Before coming to class, make sure you can:

* \[ \] Import pandas as pd without errors.  
* \[ \] Load the ex1.csv file using pd.read\_csv('data/ex1.csv').  
* \[ \] Explain what a CSV file is.

## **🔜 What's Next?**

In our **3-hour class session**, we will:

1. **Ingest** messy data from text files and databases.  
2. **Clean** a real Singapore HDB resale price dataset.  
3. **Discover** which factors actually drive flat prices using statistics.

**Bring to Class:**

* ✅ Laptop with environment set up.  
* ✅ The downloaded data files in a known folder.



### Foundation

- [Beginner's Guide to Statistics](https://www.analyticsvidhya.com/blog/2021/08/a-beginners-guide-to-statistics-for-machine-learning/)
- [Introduction to Regular Expressions in Python](https://developers.google.com/edu/python/regular-expressions)
