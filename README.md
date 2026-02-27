# Secure Password Policy Testing on a Sample Application

This project focuses on evaluating password security mechanisms in a web application environment. The goal is to identify weaknesses in authentication controls, password policies, and storage techniques, and recommend improvements to enhance system security.

The project was performed using a vulnerable sample application to simulate real-world security testing scenarios.

---

## 📌 Project Objectives

- Evaluate password complexity enforcement mechanisms
- Test authentication systems against brute-force attacks
- Analyze password storage algorithms
- Assess hash strength using password cracking tools
- Identify vulnerabilities in authentication mechanisms
- Recommend security improvements for better protection

---

## 🛠️ Tools Used

- Burp Suite Community Edition – Intercepting and analyzing login requests
- Hydra – Automated brute-force password testing
- Hashcat – Password hash strength analysis
- OWASP Juice Shop – Vulnerable sample web application
- Kali Linux – Security testing environment
- Docker – Application deployment

---

## ⚙️ Methodology

The project was conducted in multiple phases:

1. Deploying a sample web application locally using Docker
2. Testing password complexity during account creation
3. Intercepting authentication requests using Burp Suite
4. Performing brute-force testing using Hydra and Burp Intruder
5. Analyzing password hashing algorithms
6. Evaluating hash strength using Hashcat
7. Identifying vulnerabilities and proposing mitigation strategies

---

## 🔍 Key Findings

The following security weaknesses were identified:

- Lack of brute-force protection
- No account lockout mechanism
- Absence of CAPTCHA after failed login attempts
- Unlimited login attempts allowed
- Potential weak password acceptance

However, password storage using **bcrypt hashing** was implemented securely.

---

## 🔐 Hashing Analysis

The project compared password hashing techniques:

- **bcrypt (Secure)**  
  - Uses salting  
  - Computationally expensive  
  - Resistant to rainbow table attacks  

- **MD5 (Weak)**  
  - Cracked instantly using Hashcat  
  - Not suitable for secure password storage  

This demonstrates the importance of modern hashing algorithms in application security.

---

## ✅ Security Recommendations

- Implement account lockout after multiple failed login attempts
- Add CAPTCHA after repeated authentication failures
- Apply rate limiting to login endpoints
- Enforce strong password complexity policies
- Enable Multi-Factor Authentication (MFA)
- Monitor suspicious login activity
- Continue using strong hashing algorithms like bcrypt or Argon2

---

## 📄 Project Report

The complete project report is available in this repository:

**Secure_Password_Policy_Testing_on_a_Sample_Application.pdf**

---

## 🎯 Conclusion

This project highlights the importance of strong authentication protections and secure password storage mechanisms. While bcrypt hashing provides strong protection, insufficient login defenses expose applications to brute-force attacks. Implementing proper security controls significantly improves overall system resilience.

---

## 👨‍💻 Author

MEDARI BHARATH KUMAR  
Cyber Security Student  
