# 🛒 Akakçe Test Automation Project

![Java](https://img.shields.io/badge/Java-21-orange?style=for-the-badge&logo=java)
![Selenium](https://img.shields.io/badge/Selenium-4.36.0-green?style=for-the-badge&logo=selenium)
![TestNG](https://img.shields.io/badge/TestNG-7.11.0-red?style=for-the-badge)
![Maven](https://img.shields.io/badge/Maven-3.2.5+-blue?style=for-the-badge&logo=apache-maven)

**Automated GUI Testing Framework for Akakçe (akakce.com) E-commerce & Comparison Platform**

[Demo Site](https://www.akakce.com/)

## 📋 About The Project

This project is a functional GUI test automation framework built for the [Akakçe](https://www.akakce.com/) platform. Utilizing **Selenium WebDriver** and **TestNG**, the project focuses on systematically validating user creation, session authentication, and profile tracking workflows.

### ✨ Key Features

- ✅ Requirement-mapped automation tracking from user story to code execution
- ✅ Organized component separation adhering to test automation principles
- ✅ Unified configuration architecture to isolate target environmental values
- ✅ Automated execution logs tracking test framework outcomes

## 🛠️ Tech Stack

| Technology | Version | Purpose |
|:-----------|:--------|:--------|
| **Java** | 21 | Programming Language |
| **Selenium WebDriver** | 4.36.0 | Browser Automation |
| **TestNG** | 7.11.0 | Test Framework & Management |
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
This project implements the Page Object Model (POM) design pattern, which provides:

* Better code organization - Explicit demarcation between functional test execution scripts and UI component location selectors.

* Reusability - Centralized interaction workflows and common web element strategies abstracted into reusable base helper classes.

* Maintainability - Structural application frontend UI updates can be addressed single-pointedly within independent web element layers without breaking test verification code.

* Readability - Test scenarios maintain high semantic clarity, reflecting programmatic operations instead of raw driver query selectors.

📊 Test Reporting
The framework integrates TestNG's built-in assertion engines and execution output handling to deliver concise, tabular status summaries:

* Success and failure distribution metrics gathered across the user story suites.

* Stacktrace documentation logs capture error vectors, failure points, and element visibility states during automated test cycles.

* Step execution tracking measures transaction duration for critical workflows such as account deletion and customer registration forms.
