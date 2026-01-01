# Certificate Decoder

**Easily Decode and Inspect SSL/TLS Certificates**

🔗 **Try it Live:**  
https://sslchecktool.com/tools/certificate-decoder/

---

##  What It Does

The **Certificate Decoder** allows you to inspect all the details embedded inside an SSL/TLS certificate in a clear, human-readable format.

It supports common certificate formats such as:

- PEM
- DER
- PFX / PKCS#12

This tool is especially useful for verifying certificate details **before installation** or while **troubleshooting SSL/TLS issues**.

---

##  What You’ll See When You Decode a Certificate

After decoding, the tool displays the following information:

- **Subject / Common Name (CN)**
- **Issuer** (Certificate Authority that issued the certificate)
- **Validity Period**
  - Not Before (start date)
  - Not After (expiry date)
- **Serial Number**
- **Signature Algorithm**
- **Public Key Algorithm and Key Size**
- **Subject Alternative Names (SANs)**
- **Extensions**
  - Key Usage
  - Extended Key Usage
  - Other X.509 extensions

---

## What This Helps You Verify

Using the decoded output, you can confirm that your certificate:

- Belongs to the **correct domain**
- Is **currently valid** and not expired
- Contains the **required SAN entries**
- Uses the **expected key size and algorithm**
- Is signed by the **correct Certificate Authority**

---

## How to Use the Certificate Decoder

1. Paste your certificate into the input field  
   (PEM, DER, or PFX format supported)
2. Click **Decode Certificate**
3. Instantly review all decoded certificate details

---

## 📄 Example PEM Certificate Format

```text
-----BEGIN CERTIFICATE-----
MIIF...
-----END CERTIFICATE-----
