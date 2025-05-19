Added incident report for screenshot rendering issue (2025-05-18)

# INCIDENT REPORT: Screenshot Rendering Issue in GitHub Repository

**Repository:** [CyberSecFale_Google-Cloud-Cybersecurity-Labs](https://github.com/CyberSecFale/CyberSecFale_Google-Cloud-Cybersecurity-Labs)  
**Reported By:** BOBBY [Abbiu] FⱯLERO  
**Date of Incident:** Sunday, May 18, 2025  
**Time Resolved:** 11:18 PM CDT  
**Severity Level:** Low  
**Status:** ✅ Resolved

---

## 🧾 Summary

An issue was identified in which uploaded screenshots were not rendering properly in `README.md` and `lab_screenshots.md` within the GitHub repository. The issue was tied to incorrect Markdown image paths and case-sensitive filename mismatches.

---

## 🛠️ Root Cause

- Screenshots were uploaded to the repository under a `screenshots/` directory.
- Markdown links pointed to either incorrect file names (e.g., wrong case like `Screenshot.PNG` instead of `screenshot.png`) or misconfigured relative paths.
- GitHub is **case-sensitive** and requires **accurate relative paths** for Markdown to render images correctly.

---

## 🔍 Timeline of Events

| Time (CDT) | Event |
|------------|-------|
| 10:34 PM   | Observed broken image icons in Markdown preview. |
| 10:42 PM   | Began troubleshooting by reviewing Markdown syntax. |
| 10:50 PM   | Verified file names and paths via GitHub file tree. |
| 11:02 PM   | Confirmed mismatch in file names and relative links. |
| 11:10 PM   | Corrected image links in both `README.md` and `lab_screenshots.md`. |
| 11:18 PM   | Verified that screenshots rendered successfully across browsers. |

---

## ✅ Resolution Steps

1. Created a `screenshots/` directory at the repository root.
2. Uploaded the screenshots via GitHub's “Upload files” tool.
3. Verified filenames were lowercase and matched Markdown syntax exactly.
4. Used the following relative Markdown syntax:
   ```markdown
   ![Lab Screenshot](screenshots/screenshot_part1.png)

📘 Lessons Learned
Always double-check case sensitivity in filenames — GitHub treats Screenshot.png and screenshot.png as different.

Use relative paths when linking to local files for portability across branches and forks.

Preview your README.md after every major file update, especially when embedding media.

Create fallback error messages in case an image fails to load, like: ![Screenshot - may not load if file name is incorrect](screenshots/screenshot1.png)

🧠 Preventive Actions
A dedicated guide was created: How to Add and Link Screenshots in a GitHub Repository.
Repository structure now includes: /screenshots
/guides
README.md
lab_screenshots.md
incident_report_2025-05-18.md

