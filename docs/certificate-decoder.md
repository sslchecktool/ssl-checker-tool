# Certificate Decoder

**Decode and inspect SSL/TLS certificates**

🔗 Live Tool: https://sslchecktool.com/tools/certificate-decoder/

##  What It Does

A **Certificate Decoder** takes your SSL/TLS certificate (in formats like PEM, DER, or PFX) and shows all the information stored inside it in **human-readable form**. This is essential for verifying that your certificate contains the correct data before installation or troubleshooting. :contentReference[oaicite:1]{index=1}

##  What You’ll See When You Decode a Certificate

When you decode a certificate, the tool shows:

- **Subject / Common Name (CN)**
- **Issuer (CA that signed the certificate)**
- **Validity Period**
  - Not Before (start date)
  - Not After (expiry date)
- **Serial Number**
- **Signature Algorithm**
- **Public Key Algorithm and Key Size**
- **Subject Alternative Names (SANs)**
- **Extensions (Key Usage, Extended Key Usage, etc.)** :contentReference[oaicite:2]{index=2}

This helps you verify that your certificate is:
- Issued to the correct domain
- Valid for the correct period
- Contains the right SAN entries
- Signed by the expected certificate authority

##  How to Use

1. Paste your certificate text (PEM / DER) into the input box.
2. Click **Decode Certificate**.
3. Review the displayed details.

> Certificates in PEM format will look like:
>
> ```
> -----BEGIN CERTIFICATE-----
> MIIF...
> -----END CERTIFICATE-----
> ```

##  Why It Matters

Decoding certificates is useful when:
- You want to **confirm certificate contents**
- You are troubleshooting certificate installation issues
- You need to validate information before renewing or issuing certificates
- You want visibility into SAN entries and algorithms used

Verifying this information helps prevent misconfigurations and ensures a smoother SSL/TLS deployment.

 
