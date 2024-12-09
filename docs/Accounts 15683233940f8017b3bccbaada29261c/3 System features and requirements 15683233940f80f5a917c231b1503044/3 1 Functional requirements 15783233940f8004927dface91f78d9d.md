# 3.1 Functional requirements

Here are the core **functional requirements** for the **Accounts** project, detailing the specific actions the system should be able to perform:

### **1. Account Management**

- **FR1.1**: The system must allow users to add new financial accounts (e.g., checking, savings, credit card) with the option to specify the account type and initial balance.
- **FR1.2**: The system must allow users to edit the details of existing accounts, such as account name, account type, or balance.
- **FR1.3**: The system must allow users to delete financial accounts, with a confirmation prompt to prevent accidental deletion.
- **FR1.4**: The system must display a list of all accounts associated with the user, showing essential information like account name, type, and balance.

### **2. Payment Tracking**

- **FR2.1**: The system must allow users to log individual payments, including details such as the payment amount, payment date, and associated account.
- **FR2.2**: The system must allow users to categorize payments (e.g., utilities, rent, groceries, entertainment).
- **FR2.3**: The system must display a history of all recorded payments, with options to filter by payment date, category, or associated account.
- **FR2.4**: The system must allow users to edit or delete individual payments, should there be any mistakes or changes.

### **3. Debt and Bill Management**

- **FR3.1**: The system must allow users to input debts, including the debt amount, due date, and the associated account.
- **FR3.2**: The system must allow users to input recurring bills (e.g., monthly subscriptions, rent), including amount and due date.
- **FR3.3**: The system must send notifications to users when a bill or debt is due, based on their preferences (e.g., email, app notifications).
- **FR3.4**: The system must allow users to mark bills and debts as paid, updating the balances of associated accounts accordingly.
- **FR3.5**: The system must provide a view to track all outstanding debts and unpaid bills, with clear indicators of amounts due.

### **4. Dashboard and Financial Insights**

- **FR4.1**: The system must provide a dashboard that shows a summary of all financial accounts, including total balances, total payments, total debts, and upcoming bills.
- **FR4.2**: The dashboard must display graphical representations (e.g., pie charts, bar graphs) of spending categories, balances, and trends over time.
- **FR4.3**: The system must allow users to view and compare the financial status of multiple accounts on the dashboard.

### **5. User Authentication and Security**

- **FR5.1**: The system must require users to create an account by providing a unique email address and password.
- **FR5.2**: The system must allow users to securely log in using their email and password.
- **FR5.3**: The system must implement session management, keeping users logged in until they log out or their session expires.
- **FR5.4**: The system must allow users to reset their passwords through a secure process (e.g., email verification).
- **FR5.5**: The system must store user passwords securely using modern encryption techniques (e.g., bcrypt).

### **6. Reminders and Notifications**

- **FR6.1**: The system must send notifications to users for upcoming bill payments or debt due dates.
- **FR6.2**: The system must allow users to choose their preferred notification method (e.g., email, in-app) and frequency (e.g., daily, weekly).
- **FR6.3**: The system must allow users to enable or disable notifications for specific types of bills or debts.
- **FR6.4**: The system must provide users with a notification history, showing past reminders and notifications sent to them.

### **7. Data Backup and Recovery**

- **FR7.1**: The system must back up user data regularly to prevent loss in case of system failure or errors.
- **FR7.2**: The system must allow users to restore their data from a backup in case of accidental deletion or corruption.
- **FR7.3**: The system must log backup and restore events for security and auditing purposes.