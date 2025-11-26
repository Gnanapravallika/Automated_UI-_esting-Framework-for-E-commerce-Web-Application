# Automated_UI-_esting-Framework-for-E-commerce-Web-Application

This project is a **Selenium-based UI automation framework** built using **Python** and **PyTest** to test core user flows of an e-commerce web application.

It focuses on:

-  Login testing  
-  Product search testing  
-  Add to cart testing  
-  HTML report generation  
-  Screenshot capturing on failures  

The goal is to simulate **real-world QA work** that a tester would do for an e-commerce or online shopping product.

##  Objectives

- Automate critical user journeys in an e-commerce web app (login → search → add to cart).
- Build a **structured, reusable test framework** using the **Page Object Model (POM)**.
- Generate **HTML reports** for test execution.
- Capture **screenshots automatically** when test cases fail.

##  Tech Stack

- **Language:** Python  
- **UI Automation:** Selenium WebDriver  
- **Test Runner:** PyTest  
- **Reporting:** pytest-html  
- **Driver Management:** webdriver-manager  
- **Design Pattern:** Page Object Model (POM)  

##  Project Structure

```text
project-root/
├── pages/
│   ├── base_page.py          # Common reusable methods
│   ├── home_page.py          # Home / landing page actions
│   ├── login_page.py         # Login page actions
│   ├── search_page.py        # Product search and add-to-cart
│   └── cart_page.py          # Cart validation
├── tests/
│   ├── test_login.py         # Login positive & negative tests
│   └── test_search_add_to_cart.py  # Search + add-to-cart test
├── utils/
│   └── helpers.py            # Screenshot helper
├── screenshots/              # Screenshots captured on failures
├── reports/                  # HTML test reports
├── config.py                 # Config values (URL, test credentials)
├── conftest.py               # PyTest fixtures (driver, hooks)
├── requirements.txt          # Python dependencies
└── README.md                 # Project documentation
