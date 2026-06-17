# 🛒 Akakçe Test Automation Project

![Java](https://img.shields.io/badge/Java-21-orange?style=for-the-badge&logo=java)
![Selenium](https://img.shields.io/badge/Selenium-4.36.0-green?style=for-the-badge&logo=selenium)
![Maven](https://img.shields.io/badge/Maven-3.2.5+-blue?style=for-the-badge&logo=apache-maven)

**Automated GUI Testing Framework for Akakçe (akakce.com) E-commerce & Comparison Platform**

[Demo Site](https://www.akakce.com/)

## 📋 About The Project

This project is a functional GUI test automation framework built for the [Akakçe](https://www.akakce.com/) platform. Utilizing core **Java** logic and **Selenium WebDriver**, the project focuses on systematically validating user creation, session authentication, and profile tracking workflows through sequential automated scripts.

### ✨ Key Features

- ✅ Requirement-mapped automation tracking from user story to code execution
- ✅ Sequential test execution design built directly upon core Selenium capabilities
- ✅ Unified configuration architecture to isolate target environmental values
- ✅ Automated execution console outputs tracking framework outcomes

## 🛠️ Tech Stack

| Technology | Version | Purpose |
|:-----------|:--------|:--------|
| **Java** | 21 | Programming Language |
| **Selenium WebDriver** | 4.36.0 | Browser Automation |
| **Maven** | 3.2.5+ | Build & Dependency Management |

## 📝 Test Scenarios (User Stories)

The project covers 7 comprehensive user stories mapped exactly to the implemented codebase:

| ID | User Story | Description |
|:---|:-----------|:------------|
| 🔐 **US101_UserAccountCreation** | User Account Creation | Validates successful sign-up and verifies form checks under missing input vectors |
| 🛡️ **US102_AccountVerificationCheck** | Account Verification Check | Validates profile metadata display and active authentication status checks |
| 🚪 **US103_LogOut** | Log Out | Asserts clean user session termination and verified UI page redirection |
| 🔑 **US104_Login** | Login | Verifies successful web portal authentication under valid active credentials |
| 📋 **US105_OrderListCheck** | Order List Check | Inspects past purchase lists, profile history elements, and order logs tracking |
| ✉️ **US106_MessageBoxCheck** | Message Box Check | Verifies messaging component interfaces and customer service panel routing |
| 🗑️ **US107_DeleteAccount** | Delete Account | Validates successful profile clearance and password security boundary failure points |

## 📁 Project Structure

```text
AKAKCE_PROJECT_SELENYUM1/
│
├── 📄 pom.xml                          # Maven configuration
├── 📄 README.md                        # Project documentation
│
└── src/
    └── test/
        └── java/
            ├── US101_UserAccountCreation/
            ├── US102_AccountVerificationCheck/
            ├── US103_LogOut/
            ├── US104_Login/
            ├── US105_OrderListCheck/
            ├── US106_MessageBoxCheck/
            ├── US107_DeleteAccount/
            │
            └── utility/                # Utility and driver configuration classes
```
⚙️ Configuration
Test execution parameters are centralized inside the project configuration structure within the src/test/resources/ directory paths. This design ensures that target system parameters—including primary site URLs, credential properties, and driver implicit timeout constraints—remain detached from core functional evaluation code.

🏗️ Design Pattern
This project implements structural separation concepts, which provides:

🎯 Better code organization - Explicit demarcation between functional test execution scripts and UI component interaction logics.

🔄 Reusability - Centralized driver instantiation workflows and common web element synchronization strategies abstracted into reusable utility helper classes.

🛡️ Maintainability - Frontend UI updates can be addressed within consolidated element identifier layers without altering the underlying transaction test steps.

📖 Readability - Test scenarios maintain distinct semantic clarity, reflecting sequential user operations instead of scattered raw driver commands.

📊 Test Reporting
The framework integrates native Java control structures and console logging to track automation milestones:

📈 Real-time runtime logs track successful operations and validation check checkpoints across the execution path.

📋 Stacktrace console summaries capture error vectors, failure points, and element visibility states during automated execution cycles.

⏱️ Basic execution flow analysis captures duration boundaries for critical workflows such as account deletion and customer registration forms.
