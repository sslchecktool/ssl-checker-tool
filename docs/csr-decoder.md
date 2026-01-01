# CSR Decoder

**Easily Decode and Review Your Certificate Signing Requests (CSR)**

🔗 **Try it Live:**  
https://sslchecktool.com/tools/csr-decoder/

---

## 🧠 What It Does

A **CSR (Certificate Signing Request)** is a block of encoded text that contains your **public key** and identifying information such as your **domain name, organization, and country**.

This file is submitted to a **Certificate Authority (CA)** when requesting an SSL/TLS certificate.

The **CSR Decoder** allows you to instantly inspect the contents of your CSR in a **clear, human-readable format**, helping you verify all details before submission.

---

## 🔍 What You’ll See When You Decode a CSR

Once decoded, the tool displays key CSR information including:

- **Subject / Common Name (CN)**
- **Organization (O)**
- **Country (C)**
- **Public Key Type** (RSA or ECC)
- **Key Length**
- **Subject Alternative Names (SANs)**
- **Signature Algorithm**

---

## ✅ What This Helps You Verify

Decoding your CSR helps confirm that:

- The **domain name** is correct
- Organization and country details are accurate
- The **key type and key size** meet security requirements
- Required **SAN entries** are present
- The CSR is ready for submission to a Certificate Authority

---

## 🚀 How to Use the CSR Decoder

1. Paste your CSR text into the input field  
2. Click **Decode**
3. Review the decoded details, including:
   - Subject
   - Public Key
   - Algorithm
   - SANs
4. Confirm everything is correct before issuing your SSL certificate

---

## 🛡️ Example CSR Format

```text
-----BEGIN CERTIFICATE REQUEST-----
MIIB...
-----END CERTIFICATE REQUEST-----
