# 🏦 DSA Bank Simulator (C++ Project)

Welcome to the **DSA Bank Simulator**, a C++-based command-line application that models a functional bank system with multiple ATMs. This project integrates core data structures, object-oriented programming concepts, and Standard Template Library (STL) components to simulate real-world banking operations.

---

## 📚 Overview

This project offers a simulated banking environment operating in **two modes**:

1. **Banking Mode** – For bank-level operations like account management and ATM control.
2. **ATM Mode** – Mimics the experience of using an ATM for basic customer transactions.

Users can switch between these two modes using specific keyboard commands.

---

## 💡 Features

### 🏦 Banking Mode

Use command `Z` to enter or exit this mode.

| Command | Operation                        |
| ------- | -------------------------------- |
| S       | Start/open the bank              |
| O       | Create a new account             |
| B       | Check account balance            |
| W       | Withdraw money                   |
| D       | Deposit money                    |
| C       | Close an account                 |
| A       | Activate an ATM                  |
| U       | Unlock an ATM                    |
| P       | View all account details         |
| I       | Apply interest to all accounts   |
| E       | Exit system and close all files  |

### 🏧 ATM Mode

Available after activating an ATM.

| Command | Operation              |
| ------- | ---------------------- |
| X       | Change account PIN     |
| F       | Transfer funds         |
| B       | Balance inquiry        |
| W       | Cash withdrawal        |
| M       | Mini statement         |

🔄 **Persistent Storage**: All account and transaction details are saved to files and automatically restored on the next run.

---

## 🛠 Tech Stack

- **Language:** C++ (OOP, File Handling, STL)
- **Build Tool:** GNU Make

---

## 🚀 Getting Started

### 🔧 Clone the Repository

```bash
git clone https://github.com/RaghavRanjeet/Bank.git
