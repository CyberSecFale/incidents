# INCIDENT REPORT: Python Debugging Practice – Coursera Lab

**Lab Name:** Exemplar: Debug Python Code  
**Platform:** Google Cybersecurity Certificate (Coursera)  
**Completion Date:** May 18, 2025  
**Reported by:** BOBBY [Abbiu] FⱯLERO  
**Severity of Errors:** Mixed (Syntax, Logic, Exceptions)  
**Status:** ✅ Fully Resolved

---

## 🔍 Lab Summary

This lab focused on identifying and fixing errors in Python code. As a security analyst, ensuring the reliability of automated scripts is essential. Debugging errors like incorrect syntax, logic flaws, or runtime exceptions can directly impact threat detection, data parsing, or response mechanisms.

---

## 🧪 Lab Tasks Overview

| Task | Description | Issue Type | Resolution |
|------|-------------|------------|------------|
| 1    | Fix `for` loop error | **Syntax Error** | Added missing `:` after `for` statement |
| 2    | Clean up user list syntax | **Syntax Error** | Closed missing quote and added comma |
| 3    | Print message in uppercase | **Syntax Error** | Added missing closing parenthesis |
| 4    | Validate approved user | **Syntax + Name Error** | Fixed `==`, corrected indentation, and corrected variable name |
| 5    | Check if username is last in list | **Index Error (Exception)** | Corrected index to `4` (not `5`) |
| 6    | Read IP addresses from file | **Syntax + Exception** | Fixed `:` in `with` statement, used `ip_addresses.split()` correctly |
| 7    | Match OS to patch schedule | **Logic Error** | Corrected list index usage in conditionals |

---

## ⚠️ Errors Encountered

- **Syntax Errors**: Missing `:`, incorrect indentation, unclosed strings or parentheses
- **Exceptions**: `IndexError`, incorrect method use like `split.ip_addresses()`
- **Logic Errors**: Mismatch between expected vs. actual outcomes due to wrong index values or condition ordering

---

## 🔧 Remediation Steps

1. Ran each code block independently to isolate errors.
2. Applied **Python debugging best practices**: fix one issue at a time, test after each fix.
3. Used `.split()` properly after reading from text files.
4. Corrected variable naming issues and ensured consistency.
5. Verified list indexing and ensured proper logic flow.

---

## 🧠 Key Takeaways

- **Python reads top-down** — always resolve the **first** error shown before moving forward.
- Syntax errors often involve missing punctuation like `:` or `,`.
- Exceptions are usually caused by misused methods or bad data inputs.
- Logic errors are the most deceptive — code may run, but output is incorrect.
- Debugging requires attention to detail, understanding of Python’s rules, and patience.

---

## 📁 Stored In Repository

- [CyberSecFale_Google-Cloud-Cybersecurity-Labs](https://github.com/CyberSecFale/CyberSecFale_Google-Cloud-Cybersecurity-Labs)
- File Path: `incidents/incident_report_2025-05-18_debug-python.md`

---

## 🐺 Filed Under

CyberWolf_001 – Python Debugging Practice  
FALE Network Solutions – Analyst Documentation Logs  
