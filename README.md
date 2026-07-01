# Task 2: Phishing Email Threat Analysis
[phishing_email.txt.txt](https://github.com/user-attachments/files/29548243/phishing_email.txt.txt)

## 🎯 Objective
To identify, dissect, and document phishing indicators and malicious traits found within a suspicious email sample.

## 🛠️ Tools & Methods Used
* Manual analysis of email structure and language
* Simulated Email Header Analysis 

## 📊 Phishing Indicator Report
* **Target Email:** `victim@yourcompany.com`
* **Spoofed Sender:** `IT Support Desk <security-alert@support-microsoft-update.com>`
* **Actual Originating Host:** `mail-attacker.com` (`203.0.113.50`)
* **Malicious URL Identified:** `http://login.microsoft.com-security-update.net/auth/login.html`

### Key Flags Found:
1. **Urgency Hook:** The email threatens immediate account lockdown within a strict 2-hour window.
2. **Domain Spoofing:** The domain used resembles Microsoft but belongs to a malicious external registration.
3. **Mismatched Routing:** The `Received` header flags an unauthorized mail server string.

## 🧠 Technical Interview Questions

### 1. What is phishing?
Phishing is a type of cyberattack where attackers send fraudulent messages—typically emails—designed to trick recipients into revealing sensitive information (like passwords or financial data) or installing malware.

### 2. How to identify a phishing email?
Phishing emails can be identified by checking for look-alike sender domains, generic greetings, urgent or threatening language, mismatched hyperlinks, suspicious attachments, and poor grammar or spelling.

### 3. What is email spoofing?
Email spoofing is a technique where an attacker alters the header of an email so that it appears to have originated from a trusted, legitimate source instead of the actual sender.

### 4. Why are phishing emails dangerous?
They are highly dangerous because they exploit human psychology rather than technical flaws. They can lead to credential theft, massive corporate financial loss, data breaches, and ransomware deployment across entire networks.

### 5. How can you verify the sender's authenticity?
Authenticity can be verified by analyzing the email headers to check the originating server IP and checking for standard email authentication protocols like SPF (Sender Policy Framework), DKIM (DomainKeys Identified Mail), and DMARC.

### 6. What tools can analyze email headers?
Free online tools like MXToolbox Email Header Analyzer, Google Admin Toolbox Messageheader, and Microsoft Remote Connectivity Analyzer can cleanly parse and break down email headers.

### 7. What actions should be taken on suspected phishing emails?
* Do not click any links or download any attachments.
* Report the email immediately using your organization's phish reporting tool or alert the SOC/IT department.
* Delete the email from your inbox completely.

### 8. How do attackers use social engineering in phishing?
Attackers use social engineering by manipulating human emotions like fear, urgency, curiosity, or greed. By creating high-pressure scenarios (like an account shutdown), they force targets to act quickly without thinking critically.
