# 🕵️‍♂️ QA Test Assignment: Calculator Validation  
**Assigned by**: Senior QA Engineer (Team Lead)  
**Priority**: P1 (Critical)  
**Due**: 48 hours  

## 📜 Scenario  
The development team has shipped a new calculator app for v2.3. The senior tester has:  
1. **Identified 3 critical requirements** ([REQ-45](), [REQ-46](), [REQ-47]())  
2. **Partially tested** the multiplication feature  
3. **Left the remaining validation** for you to complete  

---

## 🛠 Your Task  
### 1. Review the Senior Tester's Work  
✅ **Completed Tests**:  
| Test Case | Expected | Actual | Status |  
|-----------|----------|--------|--------|  
| `3 * 2`   | 6        | 1      | ❌ Fail |  

🔍 **Notes from Senior Tester**:  
> "Multiplication seems to subtract instead. Need to verify:  
> - If this affects all multipliers  
> - Edge cases (decimals, zero)"  

### 2. Complete These Untested Requirements  
| Requirement ID | Description                  | Test Cases Needed |  
|----------------|------------------------------|-------------------|  
| [REQ-45]       | Addition accuracy            | `2 + 2`, `0 + 5`  |  
| [REQ-46]       | Division functionality       | `6 / 2`, `5 / 0`  |  
| [REQ-47]       | Error handling               | `5 + `, `abc + 1` |  

### 3. File a Bug Report  
Use this template for new issues:  
```markdown
**Description**: [Brief summary]  
**Steps**:  
1. Enter: [input sequence]  
2. Click: [button]  
**Expected**: [correct behavior]  
**Actual**: [observed behavior]  
**Repro Rate**: 100%  
**Severity**: Critical/High/Medium/Low  
