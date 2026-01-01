# Key Matcher

**Easily verify if your private key, CSR, and SSL/TLS certificate belong together**

🔗 **Try it Live:**  
https://sslchecktool.com/tools/key-matcher/

---

## 🧠 What It Does

The **Key Matcher** tool helps you verify whether your SSL/TLS components are correctly paired.

It allows you to confirm if:

- A **Private Key** matches your **SSL/TLS Certificate**
- A **CSR (Certificate Signing Request)** matches your **SSL/TLS Certificate**

This is critical because an SSL/TLS certificate will **not install or function correctly** if it does not match the original private key or CSR.

---

## 🔍 What You Can Check

### 🔹 Private Key ↔ Certificate

- Confirms that the private key and certificate were generated together
- Prevents server-side SSL installation failures

### 🔹 CSR ↔ Certificate

- Ensures the certificate was issued from the correct CSR
- Helps validate renewals and reissued certificates

---

## 🚀 How to Use the Key Matcher

1. Paste your **SSL certificate**  
   (PEM or CRT format)
2. Paste your **Private Key** or **CSR**
3. Click **Match**
4. Instantly see whether the files are correctly paired

---

## 🧾 Why This Matters

When installing or renewing SSL/TLS certificates:

- Using the **wrong private key** causes installation failures
- Mismatched files often lead to errors such as:
  - *“Private key does not match certificate”*
  - Browser HTTPS or trust warnings after deployment

Checking file compatibility **before installation** saves time and avoids frustrating SSL/TLS issues — making this tool essential for:

- DevOps engineers
- System administrators
- Hosting providers
- Anyone managing SSL certificates

---

## 🛠 Manual Verification (Optional – OpenSSL)

You can also manually verify matching components using OpenSSL by comparing public key hashes.

### Extract public key from private key
```bash
openssl pkey -in private.key -pubout -outform pem | sha256sum
