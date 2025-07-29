# 🔐 OTP Verification System (Python)

An interactive **Python-based OTP verification system** that securely generates and sends a one-time password to users via email, simulating a real-world two-factor authentication process. Built using core Python libraries and Gmail's SMTP server, it highlights the importance of secure login flows and real-time identity verification.

---

## 🔍 Project Purpose

This project demonstrates how to use Python to build a secure and efficient OTP verification system that:
- Generates a **random 6-digit OTP**
- Sends OTP via **email using SMTP**
- Accepts **user input** for OTP verification
- Validates the OTP with **up to 3 retry attempts**

Ideal for learning secure programming, simulating 2FA systems, and showcasing real-world use of Python in **authentication workflows**.

---

## 🧰 Tools & Technologies

- **Python 3.x** – Core language for development  
- **NumPy / random** – OTP generation (6-digit random number)  
- **smtplib** – To send emails via Gmail's SMTP server  
- **email.mime.text (MIMEText)** – To format the OTP message  
- **getpass** – Securely receive password input from the user  
- **Google SMTP Server** – `smtp.gmail.com` used for email delivery  
- **Exception Handling** – Robust error handling for delivery and input  
<br>

---

## 📂 System Components

1. **OTP Generator**  
   Randomly generates a secure 6-digit OTP.

2. **Email Sending Module**  
   Sends the OTP to the recipient’s email via a secure SMTP session.

3. **User Input Handler**  
   Prompts the user to input the OTP they received.

4. **OTP Verifier**  
   Compares the input with the generated OTP and allows up to 3 attempts.

5. **Flow Manager**  
   Manages the full cycle: Generate OTP → Send Email → Receive Input → Validate OTP.

---

## ❓ Business Problem

Static passwords are no longer sufficient for securing user authentication. They are prone to reuse, phishing, and brute-force attacks. There's a need for a more **robust, session-based verification mechanism** that:
- Provides a secure way to verify identity  
- Prevents unauthorized access  
- Avoids password leaks  
- Simulates real-world 2FA authentication systems  
<br>

---

## 🎯 Goal of the Project

To build an **end-to-end secure login verification system** that mimics professional two-factor authentication (2FA) flows using core Python tools. The system helps:
- Enforce **session-specific access**  
- Demonstrate Python’s use in **email automation & identity verification**  
- Educate on implementing **retry logic** and **secure credential handling**  
<br>

---

## 📈 Key Features – Walkthrough

### ✅ OTP Generation & Delivery
- Secure, unique 6-digit OTP sent via Gmail SMTP  
- Uses `random` or `numpy` for generation  

### ✅ User Verification Process
- Collects OTP input from user  
- Validates with 3 retry attempts  
- Prints success/failure messages dynamically  

### ✅ Security Controls
- App passwords used instead of storing credentials  
- `getpass()` used to securely mask sensitive input  
- Exception handling included to manage failed email or invalid input  

### ✅ Modular Codebase
- Easy to maintain, test, and scale  
- Separated into clear functions for each task  
<br>

---

## 💡 Business Impact & Use Cases

- **Login Security**: Enhances protection for systems requiring identity checks  
- **2FA Simulation**: Emulates a typical second-layer authentication system  
- **User Education**: Introduces real-time authentication and secure email flows  
- **Cybersecurity Training**: Great for teaching secure coding and verification logic  
<br>

---

## 🧪 Test Scenarios

| Scenario                              | Expected Outcome                                |
|--------------------------------------|-------------------------------------------------|
| Valid Email & Correct OTP            | OTP sent and access granted on first attempt    |
| Incorrect OTP on 1st, correct on 2nd | Access granted within allowed retries           |
| All Attempts Failed                  | Access denied after 3 failed attempts           |
| Invalid Email                        | Email sending fails with appropriate error      |
<br>

---

## 🖥️ Execution Steps

1. Open the script in **Google Colab**, Jupyter Notebook, or any Python IDE  
2. Ensure packages are available: `random`, `smtplib`, `email`, `getpass`, `numpy`  
3. Run the file: `OTP_Verification_System.ipynb`  
4. Enter the sender email & app password  
5. Enter the recipient email → Check for OTP → Input in terminal  
<br>

---

## 📸 Screenshots / Demos

![OTP Screenshot](https://github.com/Payal281119/otp-verification-system-python/blob/main/Snapshot%20of%20project.png)  



## ⚠️ Notes

- Use **Gmail App Passwords** (not your main password) if 2FA is enabled  
- Never hardcode credentials in your code  
- Always use `getpass()` for security when inputting sensitive data  
<br>
