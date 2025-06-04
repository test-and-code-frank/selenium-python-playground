# 🧪 Python Selenium Test Automation Framework

This is a modular and scalable **test automation framework** built using **Python** and **Selenium WebDriver**. It follows industry best practices such as the **Page Object Model (POM)**, **data-driven testing**, and structured **setup/teardown** routines.

---

## 🚀 Features

- ✅ **Setup and Teardown**
  - Initialize and clean up browser sessions automatically.

- 🧪 **Data-Driven Testing**
  - Easily test with multiple data sets using `pytest.mark.parametrize`.

- 📌 **Assertions**
  - Validates test outcomes with clear and informative assertion messages.

- 📸 **Screenshot on Failure**
  - Captures screenshots automatically when a test fails (useful for debugging UI failures).

- 📄 **Page Object Model (POM)**
  - Encapsulates page-specific actions and locators in dedicated classes for maintainability.
- 📊 **Test Reporting**
  - This framework includes HTML test reporting via the pytest-html plugin.
  - After test execution, an HTML report is automatically generated in the results/ directory.
    
---

## ⚙️ Pre-requisites
Before running tests, ensure the following are set up:
* Install google chrome
* Python 3.11.4
* Dependencies installed `pip install -r requirements.txt`
* Chrome web driver added to path environment variable. 
* Firefox web driver added to path environment variable. 
* Verify that the webdriver on the path support your current Chrome/Firefox version

---

## 🧪 How to run the test
##### ✅ Run the entire test suite with HTML results
<pre>pytest test_suites\ -v --html="results/result.html"</pre>

##### 🔍 Run specific test cases with markers
<pre>pytest test_suites\ -v --html="results/result.html" -m <markname>`</pre>

---

## Sample test included in this repo
- **Test Invalid Login**
  - Validates user login functionality using invalid credentials.
- **Test Item Add, Update, Delete**
  - Validate behavior for adding, update and delete
    
## References
https://github.com/atlassian/dc-app-performance-toolkit/blob/master/app/selenium_ui/base_page.py
