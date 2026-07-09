# 🚀 Selenium Automation Projects

> A modular **UI Automation Framework** built using **Java**, **Selenium WebDriver**, **TestNG**, **Maven**, **Page Object Model (POM)**, **AssertJ**, **Allure Reports**, and **Log4j2** for automating multiple web applications.

<p align="center">

![Java](https://img.shields.io/badge/Java-11+-blue?logo=openjdk)
![Selenium](https://img.shields.io/badge/Selenium-WebDriver-43B02A?logo=selenium&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-Build%20Tool-C71A36?logo=apachemaven&logoColor=white)
![TestNG](https://img.shields.io/badge/TestNG-Framework-brightgreen)
![AssertJ](https://img.shields.io/badge/AssertJ-Assertions-orange)
![Apache POI](https://img.shields.io/badge/Apache%20POI-Excel%20Support-blue)
![Allure](https://img.shields.io/badge/Allure-Reports-ff69b4)
![Log4j2](https://img.shields.io/badge/Log4j2-Logging-yellow)

</p>

---

# 🗂️ Overview

This repository contains a modular **Selenium UI Automation Framework** designed to automate multiple real-world web applications using **Java**, **Selenium WebDriver**, **TestNG**, and **Maven**.

The framework follows the **Page Object Model (POM)** design pattern and emphasizes **code reusability**, **maintainability**, and **scalability** through reusable page objects, centralized driver management, retry mechanisms, screenshot capture, externalized configuration, and rich Allure reporting.

It also demonstrates **Data-Driven Testing (DDT)** using **Excel** and **JSON**, making it suitable as a reference for enterprise-style Selenium automation frameworks.

---

# ✨ Features

- ✅ Selenium WebDriver Automation
- ✅ Page Object Model (POM)
- ✅ Modular Framework Design
- ✅ Multiple Application Automation
- ✅ Data-Driven Testing (Excel & JSON)
- ✅ Centralized WebDriver Management
- ✅ Explicit Wait Utilities
- ✅ Retry Mechanism for Failed Tests
- ✅ Automatic Screenshot Capture
- ✅ TestNG Listeners
- ✅ Log4j2 Logging
- ✅ Allure Reporting

---

# 🛠️ Tech Stack

| Technology | Usage |
|------------|-------|
| Java 11+ | Programming Language |
| Selenium WebDriver | UI Automation |
| Maven | Dependency & Build Management |
| TestNG | Test Framework |
| AssertJ | Fluent Assertions |
| Apache POI | Excel Data-Driven Testing |
| JSON | Test Data Management |
| Log4j2 | Logging |
| Allure Reports | Test Reporting |
| IntelliJ IDEA | Development IDE |

---

# 🏗️ Project Structure

```text
Selenium_Automation_Projects/
│
├── .idea/                                                     # IntelliJ project files
├── .mvn/                                                      # Maven wrapper files
├── allure-report/                                             # Generated Allure report
├── allure-results/                                            # Allure execution results
├── failure_screenshots/                                       # Screenshots captured on failures
├── logs/                                                      # Execution logs
├── screenshots/                                               # Manual screenshots
│
├── pom.xml                                                    # Maven dependencies & build configuration
├── .gitignore
│
├── testNG-xmls/                                               # TestNG suite files
│   ├── testng_AmazonPage.xml
│   ├── testng_AppliToolsPage.xml
│   ├── testng_FlipkartPage.xml
│   ├── testng_PracticeTestAutomationPage.xml
│   ├── testng_SaucedemoPage.xml
│   ├── testng_SaucedemoPage_DDT_Excel.xml
│   ├── testng_SaucedemoPage_DDT_JSON.xml
│   └── testng_SaucedemoPage_E2E.xml
│
├── src/
│   ├── main/
│   │   ├── java/com.avinashsinha/
│   │   │
│   │   ├── base/
│   │   │   └── BasePage.java                                 # Common page actions
│   │   │
│   │   ├── driver/
│   │   │   └── DriverManager.java                            # WebDriver management
│   │   │
│   │   ├── pages/                                            # Page Object classes
│   │   │   ├── amazon/
│   │   │   │   ├── CartPage.java
│   │   │   │   ├── CheckoutCumLoginPage.java
│   │   │   │   ├── HomePage.java
│   │   │   │   ├── ProductPage.java
│   │   │   │   └── SearchPage.java
│   │   │   │
│   │   │   ├── appliTools/
│   │   │   │   ├── DashboardPage.java
│   │   │   │   └── LoginPage.java
│   │   │   │
│   │   │   ├── flipkart/
│   │   │   │   ├── CartPage.java
│   │   │   │   ├── CheckoutCumLoginPage.java
│   │   │   │   ├── HomePage.java
│   │   │   │   ├── ProductPage.java
│   │   │   │   └── SearchPage.java
│   │   │   │
│   │   │   ├── practiceTestAutomation/
│   │   │   │   ├── DashboardPage.java
│   │   │   │   └── LoginPage.java
│   │   │   │
│   │   │   └── saucedemo/
│   │   │       ├── BackToLoginPage.java
│   │   │       ├── BackToProductsPage.java
│   │   │       ├── CartPage.java
│   │   │       ├── ConfirmationPage.java
│   │   │       ├── InformationPage.java
│   │   │       ├── LoginPage.java
│   │   │       ├── OverviewPage.java
│   │   │       └── ProductsPage.java
│   │   │
│   │   ├── utils/                                            # Utilities
│   │   │   ├── DataReader.java
│   │   │   ├── PropertiesReader.java
│   │   │   ├── UtilExcel.java
│   │   │   └── WaitHelpers.java
│   │   │
│   │   └── resources/
│   │       ├── data.properties                               # Framework configuration
│   │       └── log4j2.xml                                    # Logging configuration
│   │
│   └── test/
│       ├── java/com.avinashsinha/
│       │
│       ├── base/
│       │   └── BaseTest.java                                 # Common test setup
│       │
│       ├── listeners/                                        # TestNG listeners
│       │   ├── RetryAnalyzer.java
│       │   ├── RetryListeners.java
│       │   └── ScreenshotListeners.java
│       │
│       └── tests/                                            # Test classes
│           ├── amazon/
│           │   └── TestAmazonPage.java
│           │
│           ├── appliTools/
│           │   └── TestAppliToolsPage.java
│           │
│           ├── flipkart/
│           │   └── TestFlipkartPage.java
│           │
│           ├── practiceTestAutomation/
│           │   └── TestPracticeTestAutomationPage.java
│           │
│           └── saucedemo/
│               ├── TestSauceDemo_LoginPage.java
│               ├── TestSauceDemo_ProductPage.java
│               ├── TestSauceDemo_CartPage.java
│               ├── TestSauceDemo_CheckoutInfoPage.java
│               ├── TestSaucedemoPage_DDT_Excel.java
│               ├── TestSaucedemoPage_DDT_JSON.java
│               └── TestSaucedemoPage_E2E.java
│
└── README.md
```

---

# 📦 Framework Components

| Component | Description |
|------------|-------------|
| **BasePage** | Common web actions shared across all page objects |
| **DriverManager** | Centralized WebDriver lifecycle management |
| **Page Objects** | UI element locators and page interactions |
| **BaseTest** | Common test setup and teardown |
| **WaitHelpers** | Explicit wait utilities |
| **RetryAnalyzer** | Retries failed test cases automatically |
| **ScreenshotListeners** | Captures screenshots on test failures |
| **Utilities** | Excel, JSON and configuration readers |
| **Application Modules** | Independent automation projects for multiple websites |

---

# 🌐 Applications Automated

| Application | Automation Coverage |
|-------------|---------------------|
| 🛒 Amazon | Product Search, Product Details, Cart & Checkout Flow |
| 🛍️ Flipkart | Product Search, Product Details, Cart & Checkout Flow |
| 👁️ Applitools Demo | Login & Dashboard Validation |
| 🧪 Practice Test Automation | Login & Dashboard Validation |
| 🛒 SauceDemo | Login, Product, Cart, Checkout, Data-Driven Testing & End-to-End Workflow |

---

# ✅ Test Coverage

| Module | Test Scenario |
|----------|---------------|
| Amazon | Search, Product Selection, Cart Flow |
| Flipkart | Search, Product Selection, Cart Flow |
| Applitools | Login Validation |
| Practice Test Automation | Login & Dashboard |
| SauceDemo | Login |
| SauceDemo | Products |
| SauceDemo | Cart |
| SauceDemo | Checkout |
| SauceDemo | Data-Driven Testing (Excel) |
| SauceDemo | Data-Driven Testing (JSON) |
| SauceDemo | End-to-End Purchase Flow |

---

# ▶️ Running Tests

Execute any TestNG suite using Maven.

### Example

```bash
mvn clean test -DsuiteXmlFile=testNG-xmls/testng_SaucedemoPage.xml
```

### Available Test Suites

| Suite | XML File |
|--------|----------|
| Amazon | `testng_AmazonPage.xml` |
| Applitools | `testng_AppliToolsPage.xml` |
| Flipkart | `testng_FlipkartPage.xml` |
| Practice Test Automation | `testng_PracticeTestAutomationPage.xml` |
| SauceDemo | `testng_SaucedemoPage.xml` |
| SauceDemo DDT (Excel) | `testng_SaucedemoPage_DDT_Excel.xml` |
| SauceDemo DDT (JSON) | `testng_SaucedemoPage_DDT_JSON.xml` |
| SauceDemo E2E | `testng_SaucedemoPage_E2E.xml` |

---

# 📊 Allure Reports

Generate the report using:

```bash
allure serve allure-results
```

<p align="center">
<img width="1100" src="https://github.com/user-attachments/assets/a21482fe-9873-48b5-a922-51b3d9516c90" alt="Allure Report">
</p>

The command launches an interactive Allure dashboard in your default browser.

---

# 👨‍💻 Author

**Avinash Sinha**

If you found this repository helpful, consider giving it a ⭐ on GitHub.

---

# 📄 License

This project is intended for **educational** and **learning purposes**.
