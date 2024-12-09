# 4.4 Nonfunctional requirements

Nonfunctional requirements describe the quality attributes of the system, including performance, security, scalability, and reliability. These requirements ensure that the system meets user expectations in terms of usability, speed, and efficiency. Below are the nonfunctional requirements for the **Accounts** project.

### **1. Performance Requirements**

**Description**:

Performance requirements define the system's responsiveness, throughput, and overall efficiency.

- **NR1.1**: **Response Time**:
    - The system should respond to user requests (e.g., logging in, viewing account details) within **3 seconds** for 95% of interactions.
    - For transaction-related operations, such as adding payments or updating account balances, the system should complete the task within **5 seconds**.
- **NR1.2**: **Throughput**:
    - The system should handle up to **1,000 concurrent users** without a noticeable degradation in performance.
    - The system should be able to process at least **500 transactions per second** for payment-related operations.
- **NR1.3**: **Data Retrieval**:
    - The system should retrieve and display account and transaction information in **less than 3 seconds** for most use cases, ensuring quick access to user data.

### **2. Availability Requirements**

**Description**:

Availability requirements focus on the system's uptime and reliability, ensuring it remains operational for users.

- **NR2.1**: **System Uptime**:
    - The system must maintain **99.9% availability** over the course of a year, meaning the system should be down no more than **8 hours and 45 minutes** per year.
- **NR2.2**: **Redundancy**:
    - The system should implement redundancy for critical services (e.g., database and payment processing) to ensure high availability and minimize downtime.
- **NR2.3**: **Disaster Recovery**:
    - The system should provide disaster recovery mechanisms, ensuring that data can be restored from backups within **4 hours** after a major system failure or outage.

### **3. Security Requirements**

**Description**:

Security requirements outline the measures needed to protect user data, prevent unauthorized access, and ensure safe transactions.

- **NR3.1**: **Data Encryption**:
    - All sensitive user data, including login credentials, account information, and payment details, must be encrypted using **AES-256** or a higher standard.
    - Data in transit between the client and server should be encrypted using **TLS 1.2** or higher to ensure secure communication.
- **NR3.2**: **Authentication and Authorization**:
    - The system must implement **multi-factor authentication (MFA)** for user login, ensuring that access to sensitive information is protected by an additional layer of security.
    - Users must have role-based access controls (RBAC) to restrict access to sensitive operations such as account deletion or payment processing.
- **NR3.3**: **Compliance with Standards**:
    - The system should comply with industry-standard security regulations and frameworks, such as **GDPR** for user privacy, and **PCI-DSS** if processing payments directly.
- **NR3.4**: **Session Management**:
    - User sessions must expire automatically after **15 minutes** of inactivity to minimize the risk of unauthorized access.

### **4. Scalability Requirements**

**Description**:

Scalability requirements define how the system will handle growth, ensuring it can scale up or down based on usage demand.

- **NR4.1**: **Horizontal Scalability**:
    - The system must be horizontally scalable, allowing additional servers to be added as the number of users and transactions grows, without affecting performance.
- **NR4.2**: **Database Scalability**:
    - The database should be able to handle an increasing amount of data and transactions, supporting **1 million users** and **10 million transactions** without degradation in performance.
- **NR4.3**: **Load Balancing**:
    - The system should implement load balancing to distribute incoming requests evenly across available servers, ensuring that no single server becomes overwhelmed.

### **5. Usability Requirements**

**Description**:

Usability requirements focus on how easy and intuitive the system is for users to interact with.

- **NR5.1**: **User Interface (UI) Accessibility**:
    - The system must adhere to **WCAG 2.1** accessibility standards, ensuring it is usable by people with disabilities, including support for screen readers and keyboard navigation.
- **NR5.2**: **Mobile Responsiveness**:
    - The system’s user interface should be fully responsive, ensuring it works seamlessly across different devices and screen sizes, including smartphones, tablets, and desktops.
- **NR5.3**: **Ease of Use**:
    - The system must have an intuitive and clean design with simple navigation, ensuring users can easily perform tasks like adding accounts, managing payments, and tracking debts without the need for extensive training.

### **6. Maintainability Requirements**

**Description**:

Maintainability requirements ensure the system can be easily updated, modified, and maintained over time.

- **NR6.1**: **Modular Architecture**:
    - The system should be designed with a modular architecture, enabling easy updates and adding new features (e.g., adding new payment methods, additional notifications) without disrupting the overall functionality.
- **NR6.2**: **Code Quality**:
    - The system should be built with clean, well-documented, and modular code that follows best practices in software development. This includes code reviews, unit testing, and integration testing to ensure the system’s stability.
- **NR6.3**: **Error Logging and Monitoring**:
    - The system must include error logging and monitoring tools to capture system issues, allowing for quick identification and resolution of problems. Logs should be stored securely and be easily accessible for troubleshooting.

### **7. Compatibility Requirements**

**Description**:

Compatibility requirements focus on how the system will interact with different platforms, devices, and third-party services.

- **NR7.1**: **Cross-Browser Compatibility**:
    - The web version of the system should work seamlessly across modern browsers (e.g., Chrome, Firefox, Edge, Safari) and ensure consistent behavior across them.
- **NR7.2**: **Mobile Platform Support**:
    - The mobile application should support both **iOS** (version 12 or higher) and **Android** (version 8 or higher), providing a consistent experience across both platforms.
- **NR7.3**: **Third-party API Integration**:
    - The system must be able to integrate smoothly with third-party APIs for services such as payments (Stripe, PayPal), email notifications (SendGrid), and user authentication (OAuth, Firebase).

### **8. Localization and Internationalization Requirements**

**Description**:

Localization and internationalization requirements ensure that the system can be used by a global audience.

- **NR8.1**: **Multilingual Support**:
    - The system should support multiple languages, including English and Spanish, with the ability to add more languages as needed.
- **NR8.2**: **Currency Formatting**:
    - The system should allow users to view their account balances, payments, and debts in their local currency, applying the appropriate currency formatting.