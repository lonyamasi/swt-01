# 🧪 Software Testing Lab 1: Calculator QA Validation

**Module**: Software Testing Fundamentals  
**Lab Duration**: 30min.
**Tools**: Browser (Chrome/Edge), GitHub (Issues tab), Calculator v2.3 (HTML)

---

## 🔍 Lab Context

You’ve joined the QA team as a junior software tester. A critical bug was found in the latest Calculator v2.3. Your task is to verify the app against its **3 core requirements** and submit any defects you find.

---

## 🎯 Learning Objectives

By the end of this lab, you will be able to:

✅ Analyze functional requirements and map them to test cases  
✅ Identify and report software bugs using a bug reporting template  
✅ Understand common testing mistakes in arithmetic logic  
✅ Use GitHub Issues for QA workflows

---
## 🚀 How to Run (VS Code Live Server)

### **Prerequisites**
- [VS Code](https://code.visualstudio.com/download) installed
- [Live Server extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)

### **Step-by-Step Guide**

1. **Clone and open the repository**:
   ```bash
   git clone https://github.com/PLP-Database-DEPT/lab-1.git
   cd lab-1
   code .

2. Open calculator.html in VS Code's Explorer (Ctrl+Shift+E), right-click, and select Open with Live Server.

---

## 📝 Scenario

Your team lead assigned you to validate Calculator v2.3. Initial testing found bugs in multiplication. You're now responsible for:  
1. Verifying **multiplication edge cases**  
2. Testing **addition, division, and error handling**  
3. Reporting all bugs via GitHub Issues

---

## 📂 Test Requirements

| Req ID  | Feature               | Examples to Test              |
|---------|------------------------|-------------------------------|
| REQ-45  | Addition Accuracy       | `2 + 2`, `0 + 5`, `3.1 + 2.2` |
| REQ-46  | Division Functionality  | `6 / 2`, `5 / 0`, `9 / 3`     |
| REQ-47  | Input Error Handling    | `5 +`, `abc + 1`, `1 ++ 1`    |

---

## ✅ Existing Bug: Multiplication

| Test Case | Expected | Actual | Status  |
|-----------|----------|--------|---------|
| `3 * 2`   | 6        | 1      | ❌ Fail |

**Senior QA Notes**:  
> "Multiplication seems to subtract instead. Please verify:  
> - Other multipliers like `5 * 0`, `1.5 * 2`  
> - Negative numbers  
> - Zero multiplication cases"

---

## 🧪 Your Tasks

### Task 1: Confirm and Extend Multiplication Testing

Create and run test cases such as:
- `5 * 5`
- `5 * 0`
- `-3 * 2`
- `1.2 * 2.5`

Document any bugs.

---

### Task 2: Validate Remaining Features

#### Addition
- Check if all additions are off by +1 (`2 + 2` = 5?)

#### Division
- Does `5 / 0` crash or show error?  
- Are decimals handled (`7 / 2` = 3.5)?

#### Error Handling
- Try invalid inputs like `1 ++ 2`  
- Type letters or incomplete expressions

---

### Task 3: Submit Bug Reports via GitHub

#### Instructions

1. Go to [GitHub Issues Tab](https://github.com/PLP-Database-DEPT/swt-01/issues)  
2. Click **“New Issue”** → Choose the **Bug Report template**  
3. Use the format below:

```markdown
**Requirement ID**: [REQ-XX]  
**Description**: [e.g., Addition gives +1 error]

**Steps to Reproduce**:  
1. Open `calculator.html`  
2. Enter: `2 + 2`  
3. Press: `=`

**Expected**: 4  
**Actual**: 5  
**Repro Rate**: 100%  
**Severity**: High

**Screenshot**:  
![Evidence](drag-and-drop-screenshot-here)
