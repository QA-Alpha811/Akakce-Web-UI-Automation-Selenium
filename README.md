# 🛒 Akakce.com E-Commerce Test Automation Project

![Java](https://img.shields.io/badge/Java-21-orange?style=for-the-badge&logo=java)
![Selenium](https://img.shields.io/badge/Selenium-4.x-green?style=for-the-badge&logo=selenium)
![Maven](https://img.shields.io/badge/Maven-3.2.5+-blue?style=for-the-badge&logo=apache-maven)

**Automated GUI Testing Framework for Akakce.com Price Comparison & E-Commerce Platform**

[Target Site](https://www.akakce.com/)

## 📋 About The Project

This repository contains a robust GUI test automation framework developed for [Akakce.com](https://www.akakce.com/), Turkey's leading price comparison and shopping platform. Built with **Java** and **Selenium WebDriver**, the framework focuses on validating critical user journey checkpoints—from initial onboarding and account security to dynamic system views and data privacy compliance (Account Deletion).

### ✨ Key Features

- ✅ **User-Story Driven Architecture:** Test cases directly mapped to business specifications and acceptance criteria.
- ✅ **End-to-End User Lifecycle:** Full validation of the user experience, including registration, secure session checks, and account teardown.
- ✅ **Dynamic UI Syncing:** Explicit waits implemented within utility classes to manage asynchronous web elements smoothly.
- ✅ **Clean Code Structure:** Modular packages grouping user stories independently to ensure high maintainability.

## 🛠️ Tech Stack

| Technology | Version | Purpose |
|:-----------|:--------|:--------|
| **Java** | 21 | Programming Language |
| **Selenium WebDriver** | 4.x | Browser Automation |
| **Maven** | 3.2.5+ | Dependency and Build Lifecycle Management |

## 📝 Test Scenarios (User Stories)

The automation suite covers 7 core user stories derived from the product verification specifications:

| ID | User Story / Feature | Description |
|:---|:-----------|:------------|
| 👤 **US_101** | User Account Creation | Validates the new user registration flow ensuring mandatory profile fields (name, email, password rules) are handled. |
| 🛡️ **US_102** | Account Verification Check | Verifies that a successfully authenticated user can view their precise registration name in the top-right profile header. |
| 🚪 **US_103** | Logout Functionality | Ensures users can securely log out and are immediately redirected to the system authentication page. |
| 🔑 **US_104** | User Login | Validates user authorization using correct credentials to persist account-specific preferences. |
| 📦 **US_105** | Order List Check | Navigates to the user dashboard to verify order history visibility or the presence of appropriate empty-state messages. |
| ✉️ **US_106** | Message Box Check | Controls the internal notification center to ensure targeted promotional campaigns and system messages render properly. |
| 🗑️ **US_107** | Account Deletion | Validates the complete deletion flow, ensuring personal data privacy by confirming correct password entry before account termination. |

## 📁 Project Structure

```text
AKAKCE_PROJECT_SELENYUM1/
│
├── 📄 pom.xml                          # Maven configuration
├── 📄 README.md                        # Project documentation
├── 📄 .gitignore                       # Git ignore configurations
│
└── src/
    └── test/
        └── java/
            ├── US101_UserAccountCreation/     # Test classes for account registration
            ├── US102_AccountVerificationCheck/ # Test classes for profile dashboard checks
            ├── US103_LogOut/                  # Test classes for session termination
            ├── US104_Login/                   # Test classes for user authentication
            ├── US105_OrderListCheck/          # Test classes for order logs
            ├── US106_MessageBoxCheck/         # Test classes for message center
            ├── US107_DeleteAccount/           # Test classes for secure profile deletion
            │
            └── utility/                       # Core configuration utilities
                └── BaseDriver.java            # WebDriver instantiation & synchronization hooks
```text
🏗️ Technical Architecture & Implementation
🎯 Modular Test Separation: Each user story is isolated in its own technical package, eliminating overlapping test impacts.

🔄 State Validation: Advanced cross-checks ensure data consistency (e.g., matching the profile display name exactly with the registration entity).

🛡️ Privacy Verification: US_107 explicitly automates security-critical backend-driven UI prompts, asserting that account deletion operations cannot occur without an active, verified session.