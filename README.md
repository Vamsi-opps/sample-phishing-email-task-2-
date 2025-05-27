# sample-phishing-email-task-2
Analyze a suspicious phishing email and identify red flags
Email Details

- **Subject**: Binance Cybersecurity  
- **From**: info@libreriacies.es  
- **To**: jdgelok@gmail.com  
- **Date**: 2023-07-25  
- **Message ID**: `<C2C067AE.1670873@libreriacies.es>`
Phishing Indicators Identified

### 1. **Suspicious Link**
- **URL Found**: `https://axobox.com/vt/wp-track.php`,in virus total scoer is 10/94
- The domain `axobox.com` is not related to Binance.
- The URL is designed to appear legitimate but could lead to credential theft or malware.
### 2. **Spoofed Sender**
- The sender claims to be from a legitimate business domain (`libreriacies.es`) unrelated to Binance.
- Email subject references Binance — a mismatch with the sender domain indicates spoofing.
- 
### 3. **Header Anomalies**
- The **SpamAssassin** score flagged:
  - Unbalanced HTML tags
  - Body mismatch between plain text and HTML
  - Truncated links
- **DKIM** signature is **missing**
- **DMARC** result: "bestguesspass" — not conclusive
- **SPF** passed, but passing SPF alone does not guarantee authenticity.

### 4. **Social Engineering Clues**
- Email subject uses the word "Cybersecurity" to evoke urgency or legitimacy.
- No content in the message promotes any real context—this aligns with common phishing tactics.

Tools Used

- [EML Analyzer (herokuapp)](https://eml-analyzer.herokuapp.com/)
- VirusTotal and URLScan integrations for domain checks
 Conclusion

This email exhibits multiple signs of phishing:
- Suspicious link to unknown domain
- Unrelated sender identity
- No valid DKIM or consistent DMARC validation
- Techniques associated with email spoofing and social engineering

**Do not click the link or engage with such emails. Report and delete them.**
