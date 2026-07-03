<div align="center">

![Header](https://capsule-render.vercel.app/api?type=waving&color=0:1a0000,50:C8102E,100:1a0000&height=220&section=header&text=FUNDAMENTAL%20BOOSTER&fontSize=42&fontColor=FFFFFF&animation=twinkling&fontAlignY=38&desc=Interactive%20Personal%20Data%20Collector%20•%20Python%20Fundamentals&descAlignY=58&descSize=16)

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=24&duration=2600&pause=700&color=C8102E&center=true&vCenter=true&multiline=true&repeat=true&width=700&height=80&lines=Variables+%2B+Data+Types+%2B+Operators;Type+Casting+%E2%86%92+int()+%2F+float();id()+%2B+type()+%E2%80%94+Peeking+Inside+Memory;Built+for+Red+%26+White+Skill+Education)](https://git.io/typing-svg)

<img src="https://img.shields.io/badge/Python-3.10%2B-3776AB?style=for-the-badge&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/Assignment-Fundamental_Booster-C8102E?style=for-the-badge" />
<img src="https://img.shields.io/badge/Status-✔_Completed-brightgreen?style=for-the-badge" />
<img src="https://img.shields.io/badge/Quality_is_our_Motto-Red_%26_White-000000?style=for-the-badge" />

<br/>

![Visitors](https://komarev.com/ghpvc/?username=PalAnghan-fundamental-booster&label=Repo%20Views&color=C8102E&style=for-the-badge)
![Last Commit](https://img.shields.io/github/last-commit/PalAnghan/Python-Fundamental-Booster-Red-White?style=for-the-badge&color=black&label=Last%20Update)

</div>

<div align="center">

### 🧭 Table of Contents

[Overview](#-project-overview) • [Live Demo](#-live-console-demo) • [Flow](#-program-flow-diagram) • [Modules](#️-core-modules) • [Code Walkthrough](#-code-walkthrough) • [Skills](#-skills-demonstrated) • [Requirements Checklist](#-assignment-requirements-checklist) • [Run](#️-how-to-run) • [Stats](#-github-analytics) • [Author](#-author)

</div>

---

## 📌 Project Overview

**Fundamental Booster** is a console-based Python application that behaves like a **live interview bot** — it greets the user, collects real personal information, and instantly reveals what's happening *under the hood* of every variable: its **data type**, its **memory address**, and how it was **type-cast** from raw text input.

This isn't just a print-statement demo. It's built to make four core Python concepts *visible and provable* on screen at runtime:

<table>
<tr>
<td width="25%" align="center">🧾<br/><b>Input & Output</b><br/><sub><code>input()</code> / <code>print()</code></sub></td>
<td width="25%" align="center">🧬<br/><b>Data Types & Operators</b><br/><sub>str · int · float</sub></td>
<td width="25%" align="center">🔁<br/><b>Type Casting</b><br/><sub><code>int()</code> / <code>float()</code></sub></td>
<td width="25%" align="center">🔍<br/><b>Introspection</b><br/><sub><code>type()</code> / <code>id()</code></sub></td>
</tr>
</table>

---
# Live Demo Video Link :
https://drive.google.com/file/d/18Cfy_pdT3Zui3kdTGjWbO2gzrn-kJMa-/view?usp=drivesdk

## 🎬 Live Console Demo

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=14&duration=1&pause=1000000&color=00FF41&center=false&vCenter=false&width=800&height=20&lines=%24+python+program.py" />

```

Welcome to the Interactive Personal Data Collector!

Please enter your name: Alice
Please enter your age: 25
Please enter your height in meters: 1.68
Please enter your favourite number: 7

Thank you! Here is the information we collected:

Name: Alice (Type: <class 'str'>, Memory Address: 140703847239568)
Age: 25 (Type: <class 'int'>, Memory Address: 9793456)
Height: 1.68 (Type: <class 'float'>, Memory Address: 140703847253232)
Favourite Number: 7 (Type: <class 'int'>, Memory Address: 9793312)

Your birth is approximately: 2001 (based on your age of 25)

Thank you for using the Personal Data Collector. Goodbye!

```

> 💡 Memory addresses change every run — that's Python's memory manager at work, and this project deliberately surfaces it instead of hiding it.

---

## 🌊 Program Flow Diagram

```

                    ┌─────────────────────────┐
                    │      Program Starts      │
                    │   Welcome Message Shown   │
                    └────────────┬─────────────┘
                                 ↓
                    ┌─────────────────────────┐
                    │     Collect Raw Input     │
                    │  name · age · height ·    │
                    │      favourite number     │
                    └────────────┬─────────────┘
                                 ↓
                    ┌─────────────────────────┐
                    │       Type Casting        │
                    │  int(input) → age          │
                    │  float(input) → height     │
                    │  int(input) → favnum       │
                    └────────────┬─────────────┘
                                 ↓
              ┌──────────────────┴──────────────────┐
              ↓                                      ↓
   ┌─────────────────────┐              ┌─────────────────────────┐
   │  Introspection Pass   │              │     Arithmetic Pass       │
   │  type(var) → data type │              │  curr_age − age = b_year │
   │  id(var)   → memory addr│              └────────────┬────────────┘
   └──────────┬───────────┘                             │
              └───────────────────┬─────────────────────┘
                                  ↓
                    ┌─────────────────────────┐
                    │   Formatted f-string      │
                    │      Summary Output        │
                    └────────────┬─────────────┘
                                 ↓
                    ┌─────────────────────────┐
                    │     Goodbye Message       │
                    └─────────────────────────┘

```

---

## ⚙️ Core Modules

| # | Module | What it does | Concepts used |
|---|---|---|---|
| 1 | 🧾 **Input Collector** | Prompts the user for name, age, height, favourite number | `input()` |
| 2 | 🔁 **Type Caster** | Converts raw string input into the correct data type | `int()`, `float()` |
| 3 | 🔍 **Introspection Engine** | Reports each variable's type and memory address | `type()`, `id()` |
| 4 | ➗ **Arithmetic Engine** | Derives an approximate birth year from current age | `-` operator |
| 5 | 🖨️ **Formatted Reporter** | Builds clean, readable output for every step | f-strings |

---

## 🔬 Code Walkthrough

<details>
<summary><b>▶ Click to expand full source — <code>program.py</code></b></summary>

```python
print("Welcome to the Interactive Personal Data Collector!")

name = input("\nPlease enter your name: ")
age = int(input("Please enter your age: "))
height = float(input("Please enter your height in meters: "))
favnum = int(input("Please enter your favourite number: "))

print("\nThank you! Here is the information we collected: ")

print(f"Name: {name} (Type: {type(name)}, Memory Address: {id(name)})")
print(f"Age: {age} (Type: {type(age)}, Memory Address: {id(age)})")
print(f"Height: {height} (Type: {type(height)}, Memory Address: {id(height)})")
print(f"Favourite Number: {favnum} (Type: {type(favnum)}, Memory Address: {id(favnum)})")

curr_age = 2026
b_year = curr_age - age

print(f"\nYour birth is approximately: {b_year} (based on your age of {age})")

print(f"\nThank you for using the Personal Data Collector. Goodbye!")
```

</details>

<details>
<summary><b>▶ Click to expand — line-by-line explanation</b></summary>

| Line(s) | Explanation |
|---|---|
| `1` | Welcomes the user and describes what the program does |
| `3` | Collects the user's **name** as a plain `str` |
| `4` | Collects **age**, immediately cast to `int` using `int()` |
| `5` | Collects **height**, immediately cast to `float` using `float()` |
| `6` | Collects **favourite number**, cast to `int` |
| `10–13` | For each variable, prints its value, its `type()`, and its `id()` (memory address) |
| `14–15` | Uses a fixed reference year (`2026`) and simple subtraction to estimate birth year |
| `17` | Prints the derived birth year using an f-string |
| `19` | Closes the program with a thank-you / goodbye message |

</details>

---

## 🎯 Skills Demonstrated

<div align="center">

![Input Handling](https://img.shields.io/badge/Input_Handling-████████████-C8102E?style=flat-square)
![Type Casting](https://img.shields.io/badge/Type_Casting-███████████-C8102E?style=flat-square)
![f--strings](https://img.shields.io/badge/f--string_Formatting-████████████-C8102E?style=flat-square)
![Memory Introspection](https://img.shields.io/badge/Memory_Introspection_(id())-██████████-C8102E?style=flat-square)
![Arithmetic Ops](https://img.shields.io/badge/Arithmetic_Operators-███████████-C8102E?style=flat-square)

</div>

- Reading and validating user input with `input()`
- Explicit type conversion using constructor functions
- Formatting dynamic, readable output with f-strings
- Inspecting Python's internal typing and memory system live
- Deriving new values from existing ones with simple arithmetic

---

## ✅ Assignment Requirements Checklist

| Requirement (per brief) | Status |
|---|:---:|
| Use `input()` to collect name, age, height, favourite number | ✅ |
| Use `print()` to guide the user through each step | ✅ |
| Store each value in an appropriately typed variable | ✅ |
| Demonstrate an arithmetic operator (birth year calculation) | ✅ |
| Use f-string / formatted output for user-friendly messages | ✅ |
| Cast input to `int` / `float` explicitly | ✅ |
| Display each variable's type using `type()` | ✅ |
| Display each variable's memory address using `id()` | ✅ |
| Welcome message + exit/goodbye message | ✅ |
| Uploaded to GitHub with a descriptive README | ✅ |

---

## ▶️ How to Run

```bash
git clone https://github.com/PalAnghan/Python-Fundamental-Booster-Red-White.git
cd Python-Fundamental-Booster-Red-White
python program.py
```

**Requirements:** Python 3.10 or higher — no external libraries needed.

---


## 👤 Author

<div align="center">

**Pal Anghan**

</div>

---

## 🤝 Connect With Me

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Pal_Anghan-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/pal-anghan/)
[![Gmail](https://img.shields.io/badge/Email-palanghan8%40gmail.com-C8102E?style=for-the-badge&logo=gmail&logoColor=white)](mailto:palanghan8@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-PalAnghan-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/PalAnghan)


</div>

---

<div align="center">

*"Quality is our Motto."* — Red & White Skill Education

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:1a0000,50:C8102E,100:1a0000&height=140&section=footer)

</div>
