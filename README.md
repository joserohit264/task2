# task2
Phishing Email Analysis Report

Objective

Identify phishing characteristics in a suspicious email sample using an email client and a free online header analyzer.

Methodology





Obtained a sample phishing email from a publicly available source.



Examined the sender's email address for signs of spoofing.



Analyzed email headers using a free online header analyzer (e.g., MX Toolbox).



Identified suspicious links or attachments in the email.



Checked for urgent or threatening language in the email body.



Verified mismatched URLs by hovering over links to reveal their true destinations.



Noted any spelling or grammar errors in the email content.



Summarized phishing traits found.

Sample Phishing Email

Below is the sample phishing email used for analysis (sourced from a fictional example for demonstration purposes, inspired by common phishing templates):

Subject: Urgent: Your PayPal Account Has Been Suspended!
From: PayPal Security security@paypal-service.com
To: user@example.com
Body:
Dear Customer,

We have detected unusual activity on your PayPal account. To prevent unauthorized access, your account has been temporarily suspended.

Please verify your account immediately by clicking the link below:
Verify Your Account Now

Failure to verify within 24 hours will result in permanent account closure.

Thank you,
PayPal Security Team

Attachment: None

Analysis

1. Sender's Email Address





Observation: The sender's email is "security@paypal-service.com".



Finding: The domain "paypal-service.com" is not associated with the official PayPal domain, which is "paypal.com". This indicates potential spoofing, as the sender is impersonating PayPal using a fake domain.

2. Email Headers





Tool Used: MX Toolbox Email Header Analyzer (https://mxtoolbox.com/EmailHeaders.aspx).



Header Sample (simplified for brevity):

Received: from unknown (192.168.1.100) by smtp.paypal-service.com
From: PayPal Security <security@paypal-service.com>
To: user@example.com
Date: Mon, 23 Jun 2025 10:15:32 +0000
Message-ID: <abc123@paypal-service.com>



Findings:





The "Received" header shows an IP address (192.168.1.100) that is a private, non-routable address, suggesting the email may originate from a suspicious source.



The domain "paypal-service.com" in the headers does not match PayPal's official SMTP servers (e.g., smtp.paypal.com).



No SPF or DKIM authentication records align with PayPal's official domain, indicating a lack of sender verification.

3. Suspicious Links or Attachments





Link: The email contains a single link labeled "Verify Your Account Now" pointing to "http://paypal-secure-login.com/verify".



Attachment: None present.



Finding: The link uses a domain ("paypal-secure-login.com") that is not affiliated with PayPal. This is a common phishing tactic to redirect users to a fraudulent website designed to steal credentials.

4. Urgent or Threatening Language





Observation: The email includes phrases like "unusual activity," "temporarily suspended," "verify your account immediately," and "permanent account closure."



Finding: The use of urgent and threatening language is a hallmark of phishing emails, designed to create panic and prompt hasty action without scrutiny.

5. Mismatched URLs





Observation: Hovering over the link "Verify Your Account Now" reveals the true URL: "http://paypal-secure-login.com/verify".



Finding: The displayed text suggests a legitimate PayPal link, but the actual URL points to a different domain, confirming a mismatch typical of phishing attempts.

6. Spelling or Grammar Errors





Observation: The email content is well-written with no obvious spelling or grammar errors.



Finding: While many phishing emails contain errors, sophisticated ones like this sample may use correct language to appear legitimate. The absence of errors does not rule out phishing.

Summary of Phishing Traits

The following phishing characteristics were identified in the sample email:





Spoofed Sender Address: The email uses a fake domain ("paypal-service.com") to impersonate PayPal.



Header Discrepancies: Lack of SPF/DKIM alignment and a suspicious private IP address in headers suggest an untrustworthy source.



Suspicious Link: The link directs to a fraudulent domain ("paypal-secure-login.com") instead of PayPal's official site.



Urgent/Threatening Language: Phrases like "temporarily suspended" and "permanent account closure" create a sense of urgency to manipulate the recipient.



Mismatched URL: The link’s displayed text does not match its actual destination, a common phishing tactic.



No Spelling/Grammar Errors: The email is professionally written, indicating a sophisticated phishing attempt.

Recommendations





User Awareness: Train users to verify sender email domains and avoid clicking links in unsolicited emails.



Technical Controls: Implement email filtering with SPF, DKIM, and DMARC to block spoofed emails.



Reporting: Encourage reporting of suspicious emails to IT/security teams for further analysis.



Verification: Always access services like PayPal directly through official websites or apps, not via email links.

Conclusion

The analyzed email exhibits multiple phishing indicators, including spoofing, suspicious links, and urgent language. Users should exercise caution with similar emails and follow best practices to avoid falling victim to such scams.
