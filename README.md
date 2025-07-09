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

## 📚 Vulnerabilities Covered

1. **SQL Injection**  
   - Used SQL payloads to bypass login and extract data  
2. **Cross-Site Scripting (XSS)**  
   - Injected malicious scripts in input fields and saw them executed  
3. **Broken Authentication**  
   - Manipulated sessions and login flow  
4. **Insecure Direct Object References (IDOR)**  
   - Accessed restricted resources by changing URL parameters  
5. **Security Misconfiguration**  
   - Exploited default settings and weak configurations  
6. **Sensitive Data Exposure**  
   - Captured sensitive info sent over unprotected channels  
7. **Broken Access Control**  
   - Escalated privileges and accessed admin functionality  
8. **Cross-Site Request Forgery (CSRF)**  
   - Triggered actions via forged requests  
9. **Using Components with Known Vulnerabilities**  
   - Identified outdated PHP modules and packages  
10. **Insufficient Logging & Monitoring**  
   - Simulated attacks that went undetected

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

Stay tuned.

---

## 📎 Credits & Resources

- **Tools Referenced**: OWASP.org, PortSwigger, DVWA documentation  

---

## 📬 Feedback

Feel free to open an issue or reach out if you have suggestions, questions, or want to collaborate.

---

## 📄 License

This project is for educational purposes only. Use responsibly.

