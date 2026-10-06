# BSW Web Application – Manual Testing Project

Manual testing of the **BSW web application** covering the UI, Login, Registration and Home page modules. The project contains **32 documented test cases** with test data, expected and actual results, pass/fail status, and the defects found during execution.

---

## Project Overview

| Item | Details |
|---|---|
| **Project name** | BSW Web Application – Manual Testing |
| **Application type** | Web application |
| **Testing type** | Manual testing (functional, UI, validation, security basics) |
| **Browser used** | Google Chrome 145 |
| **Test documentation** | Google Sheets / MS Excel |
| **Test cases** | 32 |
| **Duration** | July 2026 |

---

## Modules Covered

| Module | Test Case IDs | Test Cases | Focus |
|---|---|---|---|
| **UI / General** | TC_UI_01 – TC_UI_04 | 4 | Website load, responsiveness, logo, navbar behavior |
| **Login** | TC_LOGIN_05 – TC_LOGIN_14 | 10 | Page load, heading, placeholders, credentials, CAPTCHA, SQL injection, Reset Password |
| **Registration** | TC_REG_15 – TC_REG_24 | 10 | Form fields, field validation, mandatory fields, valid registration |
| **Home Page** | TC_HOME_25 – TC_HOME_32 | 8 | Navigation, text visibility, Buy Now button, scroll controls, footer |

**Focus areas across modules:** Website Load & UI, Responsiveness, Navigation & Scrolling, Input Validation, Security (CAPTCHA & SQL Injection).

---

## Components Tested

### 1. Navbar, Logo and Overall UI
- Website load without errors and proper display of all UI elements
- Logo clarity and alignment inside the navbar while scrolling
- Navbar staying fixed at the top while scrolling
- Layout behavior at 1366x768 and 768x1024 screen sizes

### 2. Login Page
- Page load and visibility of all UI elements
- "Login" heading, Username placeholder text, CAPTCHA label position
- Blank credentials and invalid credentials validation messages
- SQL injection input handling
- Password masking and wrong CAPTCHA handling
- Reset Password link redirection

### 3. Registration Form
- Placeholder text of First Name and Username fields
- Email, mobile number, name and DOB field validation
- Special characters and numeric values in name fields
- Mandatory field validation and blank form submission
- Password policy (minimum length)
- Registration with valid inputs

### 4. Home Page
- Home link navigation
- Visibility and contrast of page text
- Buy Now button functionality and visibility
- Up/down scroll arrows and scroll-up button (including smooth scrolling)
- Footer section display

---

## Types of Testing Performed

- **UI / GUI testing** – layout, alignment, visibility and styling
- **Functional testing** – buttons, links and navigation
- **Field validation testing** – positive and negative inputs
- **Security basics** – SQL injection input, password masking, CAPTCHA validation
- **Responsiveness testing** – different screen resolutions

---

## Test Execution Summary

| Module | Total | Pass | Fail |
|---|---|---|---|
| UI / General | 4 | 2 | 2 |
| Login | 10 | 3 | 7 |
| Registration | 10 | 0 | 10 |
| Home Page | 8 | 2 | 6 |
| **Total** | **32** | **7** | **25** |

---

## Key Defects Found

| Test Case | Module | Defect Observed |
|---|---|---|
| TC_UI_02 | UI | Layout overlaps and becomes distorted on smaller screen sizes |
| TC_UI_04 | UI | Navbar scrolls with the page instead of staying fixed |
| TC_LOGIN_06 | Login | "Login" heading is missing from the form |
| TC_LOGIN_07 | Login | Username field shows the wrong placeholder text |
| TC_LOGIN_09 | Login | No validation messages when Username, Password and CAPTCHA are blank |
| TC_LOGIN_10 | Login | No error message for invalid credentials |
| TC_LOGIN_11 | Login | SQL injection input causes an incorrect "invalid CAPTCHA" error |
| TC_LOGIN_14 | Login | Reset Password link redirects to the Registration page |
| TC_REG_16 | Registration | Invalid email format is accepted |
| TC_REG_19 | Registration | Short mobile number is accepted |
| TC_REG_21 | Registration | Weak password is accepted |
| TC_REG_22 | Registration | Valid registration fails with a DateTime error |
| TC_REG_23 / 24 | Registration | Numbers in name fields and letters in the DOB field are accepted |
| TC_HOME_27 | Home | Scroll arrows do not scroll the page |
| TC_HOME_28 | Home | Buy Now button does nothing when clicked |
| TC_HOME_30 | Home | Footer section is not visible |

**Main defect patterns:** missing input validation, UI/placeholder issues, broken navigation and buttons, and one security-related concern on the login page.

---

## Test Case Format

Every test case is documented with the following columns:

| Column | Description |
|---|---|
| Test Case ID | Unique ID (for example TC_LOGIN_09) |
| Test Scenario | What area is being verified |
| Test Case Title | Short description of the check |
| Precondition | State required before execution |
| Test Steps | Steps followed during execution |
| Test Data | Input values used |
| Expected Result | How the application should behave |
| Actual Result | What actually happened |
| Status | Pass / Fail |
| Post Condition | System state after execution |

---

## Test Case Document

- **Excel file:** `BSW_Manual_Testing_Project.xlsx` (in this repository)
- **Google Sheet:** https://docs.google.com/spreadsheets/d/1aB1qFDDEvOLTrWkHNH2M4NPOljF-bzd3kmPkizY9yi0/edit?usp=sharing

---

## Repository Structure

```
BSW-Web-Application-Manual-Testing/
├── README.md
└── BSW_Manual_Testing_Project.xlsx
```

---

## Tools Used

- Google Chrome 145
- Google Sheets / Microsoft Excel (test case and defect documentation)

---

## Author

**Ayush Jha**
- GitHub: [ayushstack-hub](https://github.com/ayushstack-hub)
- LinkedIn: [ayushjhaofficial](https://www.linkedin.com/in/ayushjhaofficial/)
- Email: ayushtech92@gmail.com
