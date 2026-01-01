# CSR Decoder

**Decode and inspect Certificate Signing Requests (CSR)**

🔗 Live Tool: https://sslchecktool.com/tools/csr-decoder/

## What It Does

A **CSR (Certificate Signing Request)** is a block of encoded text that contains your public key and identity information (domain, organization, etc.) that you send to a Certificate Authority (CA) when requesting an SSL/TLS certificate.  
Sometimes you need to *check what information is actually inside* the CSR — that’s where a CSR Decoder helps. :contentReference[oaicite:1]{index=1}

This tool decodes your CSR and displays all its fields in a clear, readable format.

## What You’ll See

When you decode a CSR, the tool shows:

- **Subject / Domain Name (CN)**
- **Organization**
- **Country**
- **Public key type (RSA / ECC)**
- **Key length**
- **SAN (Subject Alternative Names)**  
- **Signature algorithm**

These fields help you **verify that the CSR is correct** before you submit it to a CA. :contentReference[oaicite:2]{index=2}

## 🚀 How to Use

1. Paste your CSR text into the box.
2. Click **Decode**.
3. View decoded details like:
   - Issuer
   - Public key
   - Algorithm
   - SANs
   - Subject
4. Validate key details before SSL issuance.

## Why It Matters

Verifying your CSR ensures:
- Accurate domain and organization info
- Correct key type and length
- No mistakes before certificate issuance

## 🛡️ Example CSR Format
-----BEGIN CERTIFICATE REQUEST-----
MIIB...
-----END CERTIFICATE REQUEST-----


---

 

