# GitHub Repository Description

"A simple Python project that calculates Mulank (Numerology Number) from a user's date of birth using loops and basic string manipulation techniques."

---

# README.md

# Mulank Calculator

A beginner-friendly Python project that calculates a person's **Mulank (Numerology Number)** based on their date of birth.

This project demonstrates:

* String handling in Python
* Loops and conditions
* Digit extraction
* Basic numerology logic
* Function creation in Python

## What is Mulank?

In numerology, the **Mulank** is calculated by adding all digits of a person's birth date until a single digit is obtained.

### Example

Date of Birth: `24-07-2004`

Calculation:

2 + 4 + 0 + 7 + 2 + 0 + 0 + 4 = 19

1 + 9 = 10

1 + 0 = 1

Mulank = **1**

---

## Technologies Used

* Python 3
* Jupyter Notebook

---

## Project Structure

```bash
Mulank/
│
├── Mulank.ipynb
└── README.md
```

---

## How to Run the Project

### Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/Mulank.git
```

### Step 2: Open the Project Folder

```bash
cd Mulank
```

### Step 3: Run the Notebook

Open `Mulank.ipynb` in:

* Jupyter Notebook
* VS Code
* Google Colab

Run all cells.

---

## Sample Code

```python
def get_mulank(dob):
    digits = ""

    for ch in dob:
        if ch.isdigit():
            digits += ch

    total = 0

    for digit in digits:
        total += int(digit)

    while total >= 10:
        s = 0
        for digit in str(total):
            s += int(digit)
        total = s

    return total
```

---

## Sample Output

```bash
Enter Date of Birth: 24-07-2004
Mulank: 1
```

---

## Future Improvements

* Add GUI using Tkinter
* Create web version using Flask
* Add astrology/numerology predictions
* Convert into mobile app
* Add user input validation

---

## Learning Outcome

Through this project, I practiced:

* Python basics
* Problem-solving
* Functions and loops
* Working with user input
* Logic building

---

## Author

Siddhi Damkondwar

Final Year B.Tech IT Student
