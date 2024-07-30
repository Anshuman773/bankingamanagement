

# Banking System

## Introduction
This project is a simple banking system implemented in C++ that allows users to perform various banking operations such as opening an account, making deposits and withdrawals, closing accounts, and viewing account details. The data is stored persistently using file I/O.

## Features
- **Open an Account**: Create a new account with a unique account number, first name, last name, and initial balance.
- **Balance Enquiry**: Check the current balance and account details.
- **Deposit**: Add money to an existing account.
- **Withdraw**: Withdraw money from an existing account, ensuring that the minimum balance requirement is maintained.
- **Close an Account**: Close an existing account.
- **Show All Accounts**: Display the details of all accounts in the bank.

## Requirements
- C++ compiler (e.g., GCC)
- Standard Template Library (STL)
- File I/O for persistent data storage

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/banking-system.git
   ```
2. Navigate to the project directory:
   ```bash
   cd banking-system
   ```
3. Compile the project:
   ```bash
   g++ -o banking_system banking_system.cpp
   ```

## Usage
Run the executable:
```bash
./banking_system
```
Follow the on-screen prompts to use the various features of the banking system.

## Code Overview
### Account Class
This class represents a bank account with the following attributes:
- `accountNumber`: Unique identifier for the account
- `firstName`: First name of the account holder
- `lastName`: Last name of the account holder
- `balance`: Current balance in the account

Key methods:
- `Deposit(amount)`: Adds the specified amount to the account balance.
- `Withdraw(amount)`: Deducts the specified amount from the account balance, ensuring the minimum balance requirement is maintained.

### Bank Class
This class manages the collection of accounts and provides methods for performing various banking operations.

Key methods:
- `OpenAccount(fname, lname, balance)`: Creates a new account.
- `BalanceEnquiry(accountNumber)`: Retrieves the details of a specified account.
- `Deposit(accountNumber, amount)`: Deposits the specified amount into the specified account.
- `Withdraw(accountNumber, amount)`: Withdraws the specified amount from the specified account.
- `CloseAccount(accountNumber)`: Closes the specified account.
- `ShowAllAccounts()`: Displays details of all accounts.

## Data Persistence
Account data is stored in a file named `Bank.data`. The file is read at startup to load existing accounts and written at shutdown to save any changes made during the session.

## Exception Handling
The program includes basic exception handling to manage insufficient funds during withdrawal operations.

## Contributions
Contributions are welcome! Please fork the repository and create a pull request with your changes.


## Author
Anshuman Mahapatra

---

