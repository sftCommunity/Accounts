# 3. Security Requirements

**Description**:

Security requirements define how the system should protect user data and ensure privacy.

- **NFR3.1**: **Data Encryption**
    - All sensitive data (e.g., account information, payment details) should be encrypted using **AES-256** encryption both in transit (using HTTPS/TLS) and at rest.
- **NFR3.2**: **Authentication**
    - The system must support **multi-factor authentication (MFA)** for all users, especially for financial transactions, to increase security.
- **NFR3.3**: **Authorization and Access Control**
    - Only authorized users should have access to specific account data. Role-based access control (RBAC) will be implemented to ensure users can only access their own accounts and transactions.
- **NFR3.4**: **Session Management**
    - User sessions should automatically expire after **15 minutes** of inactivity to minimize the risk of unauthorized access.
    - Session tokens should be securely stored and invalidated on logout.
- **NFR3.5**: **Auditing and Logging**
    - All system activities (e.g., login attempts, account changes, transaction activities) must be logged for auditing purposes. Logs should be stored securely and accessible only to administrators.