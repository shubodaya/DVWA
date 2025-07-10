# 🔍 OWASP Top 10 Hands-On Lab with DVWA

This project is part of my ongoing journey to deepen practical cybersecurity skills by simulating both attacker and defender perspectives. After exposing a Windows 10 VM to the internet and analyzing attacks using Microsoft Sentinel, I flipped roles and explored how attackers exploit common web vulnerabilities.

In this repo, you’ll find a detailed walkthrough of how I manually tested and exploited the **OWASP Top 10 vulnerabilities** using **Damn Vulnerable Web Application (DVWA)**.

---

## 📌 What’s in This Repo

- Step-by-step breakdown of each OWASP Top 10 vulnerability
- Screenshots showing successful exploitation
- Payloads and testing methods used
- Notes on potential mitigations and what defenders can learn
- Reflections from both offensive and defensive angles

---

## 🔧 Lab Setup

- **Platform**: DVWA hosted on an intentionally vulnerable VM  
- **Tools Used**:
  - DVWA (Damn Vulnerable Web Application)
  - Burp Suite (Community Edition)
  - Kali Linux
  - Firefox Developer Edition
  - OWASP ZAP (optional)
- **Environment**: Localhost / NAT / Internet-exposed VM (depending on the test)

---

## 📚 Vulnerabilities Covered (OWASP Top 10 – 2021)

1. **A01:2021 – Broken Access Control**  
   - Accessed unauthorized pages, escalated privileges, and bypassed restrictions via IDOR and direct URL manipulation.

2. **A02:2021 – Cryptographic Failures** *(formerly Sensitive Data Exposure)*  
   - Intercepted credentials and sensitive information sent over HTTP without encryption.

3. **A03:2021 – Injection**  
   - Performed SQL Injection using crafted payloads to bypass login and extract database content.

4. **A04:2021 – Insecure Design**  
   - Explored weak security design patterns like lack of input validation and no secure defaults.

5. **A05:2021 – Security Misconfiguration**  
   - Exploited default credentials, unnecessary services, and verbose error messages.

6. **A06:2021 – Vulnerable and Outdated Components**  
   - Identified old PHP versions and insecure software packages used in the DVWA environment.

7. **A07:2021 – Identification and Authentication Failures** *(formerly Broken Authentication)*  
   - Bypassed login via brute-force and session manipulation using Burp Suite Intruder.

8. **A08:2021 – Software and Data Integrity Failures** *(partially covered)*  
   - Simulated risks from using components without verifying integrity (e.g., no signature validation).

9. **A09:2021 – Security Logging and Monitoring Failures**  
   - Executed various attacks without triggering any alerts or logs from the system.

10. **A10:2021 – Server-Side Request Forgery (SSRF)** *(manually tested if DVWA was extended)*  
   - Tested simulated scenarios where the application could be tricked into making internal requests.


---

## 📸 Screenshots

Screenshots of each exploit and attack flow are included in the `/screenshots` folder for reference, along with step-by-step instructions in the accompanying DVWA.pdf file in this repo.

---

## 🧠 Key Takeaways

- Practical exploitation solidifies theoretical knowledge  
- Small misconfigurations can lead to major breaches  
- Understanding attacker techniques sharpens defensive skills  
- Logging, monitoring, and proper access control are non-negotiable in real-world apps

---

## 🔒 Coming Next

Next phase: Implementing a **Web Application Firewall (WAF)** to defend against these attacks and analyzing its effectiveness.


---

## 📎 Credits & Resources

- **Tools Referenced**: OWASP.org, PortSwigger, DVWA documentation  

---

## 📬 Feedback

Feel free to open an issue or reach out if you have suggestions, questions, or want to collaborate.

---

## 📄 License

This project is for educational purposes only. Use responsibly.

