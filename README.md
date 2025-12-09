# BankOfDawood  
A Simple Java Banking System (Console Application)

BankOfDawood is a Java-based console banking system that simulates the core features of a real bank.  
It includes account creation, login, deposits, withdrawals, overdraft handling, transfers, currency conversion, encryption, data storage, Generate PDF statements and transaction logs.
This project demonstrates strong knowledge of OOPs concept, file handling, Java utilities, and Test Driverarchitecture.

## Features

###User Account System
- Create customer accounts
- Login using encrypted passwords (AES encryption)
- File-based storage so data stays even after restart

###Banking Operations
- Deposit money  
- Withdraw money (with overdraft control)
- Transfer between accounts
- View current balance
- Account activation/deactivation

### Transaction Logging
Every deposit or withdrawal is saved in `log.txt`:

### Currency Conversion
- Supports BHD, USD, EUR, GBP, SAR, PKR
- Implemented using `HashMap<String, Double>`
- Clean Optional-based result handling

### File Persistence
Data is stored in simple files using:
- `BufferedReader`
- `BufferedWriter`

This acts as a mini local database.

### Account Types
- **Checking Account** (allows overdraft up to –100)
- **Saving Account** (interest rate and minimum balance)

---

## OOP Concepts Used

### **Interfaces**
`Currency`  
Defines required methods for currency handling.
### **✔ Abstract Classes**
- `Account`
- `AccountTransactions`
- `Currencies`
- `Cards`

These provide shared logic to avoid repeating code.

### **✔ Concrete Classes**
- `CheckingAccount`
- `SavingAccount`
- `Customer`
- `BankOfDawood`

They contain real working implementations.

### **Encapsulation**
Private fields with getters/setters.

### **Polymorphism**
Different account types share the same base class but behave differently (e.g., overdraft logic).


##  Project Structure

src
└── com.bank
├── Account.java
├── Bank.java (interface)
├── BankAdmin.java
├── BankOfDawood.java
├── Card.java
├── CheckingAccount.java
├── Currencies.java
├── Currency.java (interface)
├── Customer.java
├── FileLoaders.java
├── fileMethods.java
├── PasswordEncryptor.java
├── PlatinumCard.java
├── SavingAccount.java
├── StandardMastercard.java
├── StartingPoint.java (main entry point)
├── TitaniumCard.java
└── User.java (interface)

Technologies Used
Java 17
AES Encryption
File I/O
Object-Oriented Programming
Streams
Optional\
Maps & Collections

##  How to Run the Project

 Right-click the file  
Click **Run 'StartingPoint.main()'**

Why StartingPoint.java?
`StartingPoint` is the **entry point** of the project.  
It:
- Loads customer & account files  
- Initializes the BankOfDawood system  
- Shows the main menu  
- Controls all user interactions  

Author
Muhammad Dawood Riaz
Bahraini Software Engineer
Java • Node.js • AWS • MySQL • MERN Stack

