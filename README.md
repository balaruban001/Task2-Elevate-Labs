# Task2-Elevate-Labs
# Phishing Email Analysis – Task 2

##  Objective

The purpose of this task is to analyze a suspicious email to identify signs of **email spoofing**, **authentication failures**, and potential **phishing tactics**.

---

##  Submission Contents

- A detailed **Word document** (`Phishing_Email_Analysis_Task2.docx`) containing:
  - Screenshots of email headers
  - SPF, DKIM, and DMARC results
  - Email body content
  - Step-by-step findings
  - Summary table of indicators

---

##  Key Analysis Checks

| Checkpoint                   | Result     | Notes                                                 |
|-----------------------------|------------|-------------------------------------------------------|
| **Sender Address**          | ⚠️ Suspicious | Not aligned with domain; uses third-party mail server |
| **SPF Authentication**      | ⚠️ Partial   | SPF passed but not aligned with From domain           |
| **DKIM Authentication**     | ❌ Failed    | DKIM signature did not verify                         |
| **DMARC Policy**            | ❌ Missing   | No DMARC policy published                             |
| **Email Links**             | ✅ None      | No links present in the email body                    |
| **Attachments**             | ✅ None      | No files were attached                                |
| **Language & Tone**         | ⚠️ Pushy     | Attempts to provoke a response with job offer claims  |

---

##  Tools Used

- Gmail/Webmail header viewer
- MXToolbox, Google Admin Toolbox
- Manual content inspection
- DNS record lookup tools

---

##  Conclusion

The email shows **multiple red flags** typical of phishing:
- Failed DKIM and DMARC checks
- Suspicious sender routing through a third-party domain
- Absence of links or attachments (to appear safe)
- Urgency and incentives (job offer) used to provoke engagement

These patterns strongly suggest the email is **spoofed and potentially malicious**.

---

##  Report Location

All findings, including screenshots and detailed notes, are documented in:

>  **Phishing_Email_Analysis_Task 2.docx**

---

##  Recommendation

- Do **not reply** to or engage with the sender.
- Report the email as phishing.
- Educate others on spotting spoofed job offer emails.

