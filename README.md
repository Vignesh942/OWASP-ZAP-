# OWASP-ZAP XSS Reflected Attack!


## ⚠️ Disclaimer  
This project is created for **educational purposes only** and aims to promote ethical cybersecurity learning.  
I do not encourage, support, or endorse any illegal hacking activities. **Testing vulnerabilities on systems you do not own or have explicit permission to test is illegal and punishable by law.**  
Use this knowledge **responsibly and ethically** in controlled environments (e.g., your own lab, bug bounty programs, or with proper authorization).  


#  CSP Misconfiguration Exploit - Web Security Testing

## 📖 Overview  
This project demonstrates how the absence of a **Content Security Policy (CSP)** can lead to **Cross-Site Scripting (XSS) attacks** and **UI modification** on a vulnerable web application.  

Using **OWASP ZAP**, I identified a **missing CSP header** and exploited it by injecting JavaScript to modify the webpage.

---

##  Tools Used  
- **OWASP ZAP** (Automated vulnerability scanning)  
- **Web Browser (Developer Console - F12)**  
- **DVWA (Damn Vulnerable Web Application) for testing**  

---

##  Vulnerability Details  
### **❌ Issue: CSP Header Not Set**
- The application does **not implement a CSP header**, making it vulnerable to **XSS attacks**.
- This allows **attackers to inject JavaScript** that can alter the page, steal data, or perform phishing attacks.

### ** Exploit - Injected JavaScript Code**
I modified the website’s UI by injecting the following script in the browser console: 
```javascript
-----------------------------------------------------------------------------------------------------------------------
document.body.innerHTML = '<h1>Hi your website has been hacked!!!!</h1>';
------------------------------------------------------------------------------------------------------------------------
```
![Screenshot 2025-02-06 205229](https://github.com/user-attachments/assets/b0b17d0b-f7fd-401f-baf9-b02ffdfee49c)![Screenshot 2025-02-06 205208](https://github.com/user-attachments/assets/3d63ee7f-1765-402f-9434-e7d5e22bc2fb)

