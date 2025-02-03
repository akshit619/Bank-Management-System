
# Bank Management System

A simple **Bank Management System** built using C++ and Object-Oriented Programming (OOP) principles, leveraging file handling to store and retrieve account data. The system allows users to create accounts, perform balance inquiries, deposit and withdraw cash, close accounts, and view all accounts. 

## Features
- **Open an Account**: Create a new bank account with an initial deposit.
- **Balance Enquiry**: Check the balance of a specific account.
- **Cash Deposit**: Deposit money into an account.
- **Cash Withdrawal**: Withdraw money from an account, ensuring a minimum balance is maintained.
- **Close an Account**: Close a specific account and remove it from the system.
- **Show All Accounts**: Display details of all accounts in the bank.

## Key Classes
1. **Cl_Accounts**: 
   - Represents a bank account with attributes like account number, client first name, last name, and balance.
   - Provides functions to deposit, withdraw, and get account details.
   - Implements file handling for account data storage and retrieval.
   
2. **Bank**:
   - Manages multiple accounts using a `map` to store them.
   - Provides functions for opening accounts, deposit/withdrawal operations, account closure, and displaying all accounts.

## Program Flow
The program presents a menu of options and allows the user to interact with the bank system by selecting one of the following operations:
1. Open an Account
2. Balance Enquiry
3. Cash Deposit
4. Cash Withdrawal
5. Close an Account
6. Show All Current Accounts
7. Quit

## Requirements
- C++ compiler with C++11 or later support.

## How to Compile and Run
1. Compile the code using your preferred C++ compiler:
   ```bash
   g++ -o BankManagementSystem BankManagementSystem.cpp
   ```
2. Run the executable:
   ```bash
   ./BankManagementSystem
   ```

## File Handling
- Account data is stored in a file named `Bank.data`.
- The system automatically reads the data from this file when it starts and writes back to it when accounts are modified or closed.

## Error Handling
- The system ensures that a minimum balance of **100** is maintained in the account after a withdrawal.
- If an attempt is made to withdraw an amount that would cause the balance to drop below this limit, an exception is thrown.

## Example Output
```
**********WELCOME TO BANK MANAGEMENT SYSTEM USING C++, OOPS AND FILEHANDLING*********
 
Select One Option Below 
    1 Open an Account
    2 Balance Enquiry
    3 Cash Deposit
    4 Cash Withdrawal
    5 Close an Account
    6 Show All Current Accounts
    7 Quit
    Enter required service option: 1

Enter First Name: John
Enter Last Name: Doe
Enter Initial Deposit: 500

Congratulations!!! Account Created
First Name: John
Last Name: Doe
Account Number: 1
Balance: 500
```

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
