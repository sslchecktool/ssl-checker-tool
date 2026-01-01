# Mail SSL Checker (SMTP / IMAP SSL & TLS Certificate Test)

**Check the SSL/TLS certificate installation for email servers (SMTP, IMAP, POP)**

🔗 Live Tool: https://sslchecktool.com/tools/mail-ssl-checker/

---

## 🧠 What It Does

The **Mail SSL Checker** verifies that your email server’s SSL/TLS certificate is correctly installed, valid, and trusted when used with common email protocols such as:

- **SMTP (Mail sending)**
- **IMAP (Mail retrieval)**
- **POP3 (Mail retrieval)**

Unlike a regular SSL certificate test for websites, email SSL/TLS certificates must also work on the specific ports and protocols used by mail services — and this tool helps confirm that they do. :contentReference[oaicite:0]{index=0}

---

## 🔍 What You Can Check

When you run a mail SSL test, the tool shows:

- **Certificate validity status**
- **Expiration date**
- **Issuer / CA (Certificate Authority)**
- **Protocol support (SSL/TLS versions)**
- **Certificate errors or misconfigurations**
- **Whether STARTTLS is correctly supported**  

STARTTLS upgrades a plain mail protocol connection (like SMTP on port 25/587) to a secure TLS session, and must work properly for secure email delivery. :contentReference[oaicite:1]{index=1}

---

## 🚀 How to Use

1. **Enter your mail server hostname** (like `mail.example.com`).  
2. Choose the **protocol** you want to test (SMTP, IMAP, POP).  
3. Enter the **port** your mail server listens on (commonly: 465, 587, 993, etc.).  
4. Click **Check SSL/TLS Certificate**.  
5. Review the results showing certificate details and any warnings.

Example common port uses:

| Protocol | Secure Port |
|----------|-------------|
| SMTP SSL | 465 |
| SMTP STARTTLS | 25 / 587 |
| IMAP SSL | 993 |
| POP3 SSL | 995 |

---

## 🎯 Why It Matters

Email security depends on having valid SSL/TLS certificates for mail services — otherwise:

- Mail clients will show certificate warnings  
- Secure connections may fail  
- STARTTLS may not function correctly  
- Outbound mail may be rejected by other servers  

This tool helps ensure **mail communications stay encrypted and trusted**. :contentReference[oaicite:2]{index=2}

---

## 🛠 Optional: How to Check via Command Line

If you want to test manually from a terminal using OpenSSL:

```bash
# SMTP with implicit SSL (port 465)
openssl s_client -connect mail.example.com:465

# SMTP STARTTLS (port 587)
openssl s_client -connect mail.example.com:587 -starttls smtp

# IMAP SSL (port 993)
openssl s_client -connect mail.example.com:993

# POP3 SSL (port 995)
openssl s_client -connect mail.example.com:995
