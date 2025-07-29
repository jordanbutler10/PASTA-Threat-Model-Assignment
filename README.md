# 👟 PASTA Threat Model – Sneaker Marketplace Mobile App

This project showcases a full **PASTA (Process for Attack Simulation and Threat Analysis)** threat model for a sneaker enthusiast mobile marketplace. The app allows users to buy and sell rare and high-demand sneakers. The threat model identifies potential security risks, system vulnerabilities, and mitigations prior to launch.

---

## 📲 Scenario Overview

As part of the cybersecurity team, I conducted a threat model for a sneaker resale mobile app using the 7-stage **PASTA framework**. The goal was to simulate attack scenarios and ensure the app is resilient to cyber threats before being released to the public.

---

## 🧠 Skills Demonstrated

- Application threat modeling  
- Attacker mindset simulation  
- Vulnerability identification and mapping  
- Security control recommendation  
- Application decomposition using data flow concepts  
- Applying the PASTA methodology in a real-world scenario

---

## 🔍 Key PASTA Stages

### 1. **Business Objectives**
- Ensure secure buyer-seller transactions  
- Protect sensitive user data (credentials, payment info)  
- Maintain system uptime during global sneaker releases

### 2. **Technology Requirements**
- React Native frontend (iOS & Android)  
- Node.js REST API backend hosted on AWS  
- MongoDB database and OAuth2.0 with JWT & MFA

### 3. **Data Flow Decomposition**
- User login and authentication  
- Product upload and image handling  
- Payment gateway integration  
- Push notification service

### 4. **Potential Threats**
- Credential stuffing to hijack seller accounts  
- Script injection through image metadata in file uploads

### 5. **System Vulnerabilities**
- No rate limiting on login endpoints  
- Unsanitized image metadata in file upload API

### 6. **Attack Tree Mapping**
- **Asset:** User Account  
  → **Threat:** Credential stuffing  
  → **Vulnerability:** No rate limiting  
  → **Impact:** Account takeover

- **Asset:** Backend Server  
  → **Threat:** Script injection  
  → **Vulnerability:** Insecure file upload  
  → **Impact:** API compromise

### 7. **Risk Mitigation**
- Implement rate limiting and lockout features  
- Enforce multi-factor authentication (MFA)  
- Sanitize and strip metadata from uploaded files  
- Use a Web Application Firewall (WAF)

---

## 📁 Files Included

- `pasta_threat_model.docx` – Completed 7-stage threat modeling document  
- `README.md` – Project overview and documentation

---

## 💡 Why This Matters

Threat modeling ensures that apps launch **secure by design**, rather than fixing vulnerabilities post-breach. This project highlights how applying structured frameworks like **PASTA** enables teams to proactively identify weaknesses, simulate attacker behavior, and implement meaningful defenses before risks turn into incidents.

---

**Author:** Jordan Butler  
**Email:** jordanbutler2300@yahoo.com  
**LinkedIn:** [Jordan Butler](https://www.linkedin.com/in/jordan-butler-168b52a2)
