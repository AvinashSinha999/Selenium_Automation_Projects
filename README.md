# 🚀 Selenium Automation Projects

> A modular **UI Automation Framework** built using **Java**, **Selenium WebDriver**, **TestNG**, **Maven**, **Page Object Model (POM)**, **AssertJ**, **Apache POI**, **Log4j2**, and **Allure Reports** to automate multiple real-world web applications.

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

This repository contains a modular **Selenium UI Automation Framework** developed to automate multiple real-world web applications using **Java**, **Selenium WebDriver**, **TestNG**, and **Maven**.

Designed around the **Page Object Model (POM)** architecture, the framework demonstrates industry-standard UI automation practices including **reusable page objects**, **centralized WebDriver management**, **explicit wait utilities**, **retry mechanisms**, **automatic screenshot capture**, **externalized configuration**, and **interactive Allure reporting**.

The project also showcases **Data-Driven Testing (DDT)** using **Excel** and **JSON**, making it a practical reference for building **scalable**, **maintainable**, and **enterprise-ready Selenium automation frameworks**.

---

# ✨ Key Features

- ✅ Selenium WebDriver Automation
- ✅ Page Object Model (POM)
- ✅ Modular Framework Architecture
- ✅ Multiple Application Automation
- ✅ Data-Driven Testing (Excel & JSON)
- ✅ Centralized WebDriver Management
- ✅ Explicit Wait Utilities
- ✅ Retry Mechanism for Failed Tests
- ✅ Automatic Screenshot Capture
- ✅ TestNG Listeners
- ✅ Log4j2 Logging
- ✅ Rich Allure Reporting

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
│   │   │   ├── appliTools/
│   │   │   ├── flipkart/
│   │   │   ├── practiceTestAutomation/
│   │   │   └── saucedemo/
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
│           ├── appliTools/
│           ├── flipkart/
│           ├── practiceTestAutomation/
│           └── saucedemo/
│
└── README.md
```

---

# 📦 Framework Components

| Component | Description |
|------------|-------------|
| **BasePage** | Provides reusable Selenium actions shared across all page objects |
| **DriverManager** | Manages the complete WebDriver lifecycle |
| **Page Objects** | Encapsulates UI locators and page interactions |
| **BaseTest** | Provides common test initialization and teardown |
| **WaitHelpers** | Implements reusable explicit wait utilities |
| **RetryAnalyzer** | Automatically retries failed test cases |
| **ScreenshotListeners** | Captures screenshots on failed test execution |
| **Utilities** | Supports Excel, JSON, configuration, and helper methods |
| **Application Modules** | Independent automation modules for multiple web applications |

---

# 🌐 Application Modules

| Application | Automation Coverage |
|-------------|---------------------|
| 🛒 **Amazon** | Product Search, Product Details, Cart & Checkout Flow |
| 🛍️ **Flipkart** | Product Search, Product Details, Cart & Checkout Flow |
| 👁️ **Applitools Demo** | Login & Dashboard Validation |
| 🧪 **Practice Test Automation** | Login & Dashboard Validation |
| 🛒 **SauceDemo** | Login, Products, Cart, Checkout, Data-Driven Testing & End-to-End Purchase Workflow |

---

# ✅ Automation Coverage

| Module | Test Scenario |
|----------|---------------|
| Amazon | Product Search & Cart Flow |
| Flipkart | Product Search & Cart Flow |
| Applitools | Login Validation |
| Practice Test Automation | Login & Dashboard Validation |
| SauceDemo | Login |
| SauceDemo | Product Catalogue |
| SauceDemo | Cart Management |
| SauceDemo | Checkout Workflow |
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

Generate and launch the Allure report using:

```bash
allure serve allure-results
```

<p align="center">
<img width="1100" src="https://github.com/user-attachments/assets/a21482fe-9873-48b5-a922-51b3d9516c90" alt="Allure Report">
</p>

The command generates and opens an interactive **Allure dashboard**, providing execution summaries, detailed logs, screenshots, and test statistics.

---

# ⭐ Repository Highlights

- ✔ Modular Selenium UI Automation Framework
- ✔ Enterprise-Style Project Structure
- ✔ Page Object Model (POM) Architecture
- ✔ Multiple Real-World Application Automation
- ✔ Data-Driven Testing (Excel & JSON)
- ✔ Centralized WebDriver Management
- ✔ Retry Mechanism & Screenshot Capture
- ✔ Explicit Wait Utilities
- ✔ TestNG Suite Execution
- ✔ Log4j2 Logging
- ✔ Rich Allure Reporting

---

# 👨‍💻 Author

**Avinash Sinha**

If you found this repository useful, consider giving it a ⭐.

---

# 📄 License

This repository is intended for **educational** and **learning purposes**.
