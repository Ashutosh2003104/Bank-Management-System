# Bank-Management-System

The Bank Management System is a Python-based console application that simulates basic banking functionalities. It allows users to perform various operations such as creating accounts, depositing and withdrawing money, viewing account details, and modifying or deleting accounts. This system utilizes file handling and serialization (`pickle` module) to manage account data persistently.

---

## Features

1. **Account Creation**
   - Users can create a new bank account by entering details like account number, name, account type (Savings or Current), and an initial deposit.

2. **Deposit and Withdrawal**
   - Allows users to deposit money into or withdraw money from their accounts.
   - Ensures that withdrawals do not exceed the current account balance.

3. **Balance Inquiry**
   - Provides the current balance of a specific account by entering the account number.

4. **Account Modification**
   - Enables users to update the account holder's name, account type, and balance for an existing account.

5. **Account Deletion**
   - Users can close an account permanently by specifying the account number.

6. **View All Accounts**
   - Displays a list of all account holders with their account numbers, names, types, and balances.

---

## Code Structure

1. **`Account` Class**
   - Represents a bank account with attributes like account number, holder's name, type, and balance.
   - Provides methods to create, display, modify, deposit, and withdraw account details.

2. **File Handling**
   - The program uses the `pickle` module to save and retrieve account details from a binary file (`accounts.data`).
   - New accounts are appended to the existing file, ensuring persistent data storage.

3. **Menu-Driven Interface**
   - Users interact with the program through a text-based menu.
   - Provides options to perform different banking operations.

---

## Example Scenarios

1. **Creating a New Account**
   - The user selects the "NEW ACCOUNT" option.
   - Enters the account details (e.g., account number, name, type, and initial deposit).
   - The account is saved in `accounts.data`.

2. **Depositing Money**
   - The user selects the "DEPOSIT AMOUNT" option.
   - Provides the account number and deposit amount.
   - The account balance is updated in the file.

3. **Withdrawing Money**
   - The user selects the "WITHDRAW AMOUNT" option.
   - Provides the account number and withdrawal amount.
   - Ensures the withdrawal amount does not exceed the available balance.

4. **Viewing Account Balance**
   - The user selects the "BALANCE ENQUIRY" option.
   - Enters the account number to view the current balance.

5. **Closing an Account**
   - The user selects the "CLOSE AN ACCOUNT" option.
   - Provides the account number, and the system deletes the account.

6. **Modifying Account Details**
   - The user selects the "MODIFY AN ACCOUNT" option.
   - Updates account details like name, type, or balance.

---

## Future Enhancements

1. **Improved Security**
   - Add authentication mechanisms like account PINs or passwords.

2. **Graphical User Interface (GUI)**
   - Transition to a GUI-based application for a better user experience.

3. **Database Integration**
   - Replace file handling with a database (e.g., MySQL) for scalable and efficient data management.

4. **Transaction History**
   - Maintain a log of all transactions for each account.

5. **Interest Calculation**
   - Automatically calculate and add interest for savings accounts periodically.

---

## Note

This application is intended for educational purposes and provides a basic implementation of banking functionalities. It does not include advanced features like concurrency, multi-user support, or security measures for sensitive data.

