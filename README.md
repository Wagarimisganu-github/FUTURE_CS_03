# Secure File Sharing System – Internship Report

---

## 📌 Executive Summary
This project presents the development of a **Secure File Sharing System** as part of the cybersecurity internship program.  
The system supports:

- Secure file upload
- AES encryption for confidentiality
- Safe encrypted storage
- Authorized download with decryption

By implementing **AES (CBC mode, 128-bit key)** and deploying the system with **Flask**, the solution ensures **end-to-end data security**. It simulates secure data transfer practices commonly used in government, finance, and cloud environments.

---

## 📖 Introduction
Secure file sharing is essential in modern infrastructures where sensitive information must be protected.  
The goal of this task was to **design and implement a secure file transfer system** that guarantees encrypted storage and controlled decryption upon authorized request.

This project demonstrates practical applications of **encryption, access control, and secure web deployment** in cybersecurity.

---

## ⚙️ Environment Setup & Exploration

### Tools & Technologies
| Tool/Library   | Purpose |
|----------------|---------|
| **Python**     | Programming language |
| **Flask**      | Web framework for building upload/download APIs |
| **PyCryptodome** | AES encryption implementation |
| **HTML**       | Frontend for file upload/download form |
| **VS Code**    | Development environment |
| **GitHub**     | Version control & code publishing |

### Features Implemented
- ✅ File upload via web form  
- ✅ AES encryption (CBC mode, 128-bit key, PKCS7 padding)  
- ✅ Encrypted file storage in secure directories  
- ✅ Download with automatic decryption  
- ✅ Auto-creation of folder paths  

### Testing Performed
1. Created a sample file (`sample.txt`).  
2. Uploaded via `http://127.0.0.1:5000/`.  
3. Verified encryption and secure storage in `/encrypted/`.  
4. Downloaded & decrypted via `/download/sample.txt.enc`.  
5. Confirmed decrypted file matched original content.  

---

## 🚨 Incident Classification by Priority

| Priority Level | Incident Description |
|----------------|-----------------------|
| **High**       | Unauthorized access attempts to encrypted folders, compromise of AES keys, insecure key storage. |
| **Medium**     | Misconfiguration of Flask routes leading to potential exposure of file paths. |
| **Low**        | User errors such as uploading unsupported file formats or repeated uploads of the same file. |

---

## 🛡️ Remediation & Recommendations

### High Priority
- Implement secure key management (e.g., **KMS**).  
- Enforce **role-based access control (RBAC)**.  
- Use **HTTPS with TLS** to secure data in transit.  

### Medium Priority
- Harden Flask app: validate routes & sanitize input.  
- Configure error handling to avoid information leakage.  

### Low Priority
- Add file format validation & upload restrictions.  
- Provide clear error messages to reduce misuse.  

---

## ✅ Conclusion
The **Secure File Sharing System** achieved its objective of providing a secure mechanism for file transfer through AES encryption and Flask deployment.  

It highlights:
- Practical use of **cryptography in cybersecurity**  
- Importance of **secure storage, encrypted communication, and access control**  
- Real-world relevance in **finance, government, and cloud environments**  

---




## 📚 References
- Daemen, J., & Rijmen, V. (2002). *The Design of Rijndael: AES – The Advanced Encryption Standard*.  
- [Flask Documentation](https://flask.palletsprojects.com)  
- [PyCryptodome Documentation](https://www.pycryptodome.org)  
- [OWASP Secure File Upload Guidelines](https://owasp.org)  

---

🔐 *Developed as part of Cyber Security Internship – Secure File Sharing System Task.*
----
## Aknowledgments
THanks to Future interns for giving this challenge
----
Reach me @
wagarimisganu12@gmail.com
