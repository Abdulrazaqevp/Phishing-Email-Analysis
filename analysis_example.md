# Full Phishing Email Analysis Example

**Sample file:** samples/sample-email.txt  
**Date analyzed:** 2025-11-15  
**Analyst:** Example Analyst  

---

## 1) Sample obtained
A fake PayPal security alert urging the user to verify their account.

## 2) Sender analysis
- From: support@paypaI-security.com  
- Domain uses uppercase 'I' instead of lowercase 'l' (common spoofing trick).

## 3) Header analysis
- SPF: FAIL  
- DKIM: NONE  
- DMARC: FAIL  
- Source IP: 95.211.124.23 (not owned by PayPal)

## 4) Links & attachments
Visible: https://paypal.com/security  
Actual: http://192.88.34.221/verify-login  
Attachment: None

## 5) Urgency
Text: “Your account will be suspended in 24 hours.”

## 6) Technical Checks
The malicious server has no HTTPS certificate.

## 7) Verdict
**Phishing — High Confidence**.
