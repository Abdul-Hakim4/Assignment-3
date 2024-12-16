## Bank Account Management System in C Using File Handling

This project demonstrates the development of a simple bank account management system in C using file handling techniques.

### Approach:

We will use a modular approach where the program features a main menu, with each option linked to a specific function. These functions will be invoked using `switch-case` statements. The key functionalities include:

1. **`account()`**: Creates a new bank account.
2. **`transfermoney()`**: Transfers money to another account.
3. **`checkbalance()`**: Displays the balance of the account.
4. **`login()`**: Handles user authentication and login.

#### Workflow:
- Start by creating a new account using the `account()` function. This will take input from the user and save the data into a file using file handling.
- Once an account is created, the user can:
  - Transfer money to another account using the `transfermoney()` function.
  - Check their account balance via the `checkbalance()` function.
- File handling is utilized to store and retrieve user data efficiently. We use structures to store account details, as they simplify data reading and writing operations.

### Implementation:

Each feature of the system is implemented as a separate module:

1. **Creating a Bank Account**:
   - Collect user information.
   - Store the data in a structure.
   - Save the structure to a file for future reference.

2. **Transferring Money**:
   - Accept the username of the recipient.
   - Locate the recipient's account in the file.
   - Update the balances of both sender and recipient accordingly.

3. **Checking Balance**:
   - Read the transaction records from the file.
   - Match the username with the records to display the correct balance.

4. **Login Functionality**:
   - Authenticate users by matching their username (entered at login) with the one stored in the file.
   - Grant access if the username matches the stored record.

### Summary:
The system leverages file handling to maintain persistent data storage, enabling the creation, modification, and retrieval of account details. The use of structures ensures data is organized and easy to manage. By combining these features, we create a functional and user-friendly bank account management system in C.
