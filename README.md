# 🔍 Email Header Analysis and Spoofing Detection Using MHA

## 🧪 Experiment No. 4

### 📚 Subject
**Digital Forensics**

### 🎯 Title

**Analyze Email Headers and Detect Email Spoofing Using MHA (Mail Header Analyzer)**

---

## 🎯 Aim

To analyze an email header using a Mail Header Analyzer (MHA) and examine the email routing information, IP addresses, SPF, DKIM, and DMARC authentication results to identify possible signs of email spoofing.

---

## 📖 Description

Email headers contain important metadata about an email's journey from the sender to the recipient.

The header can contain information such as:

- From address
- To address
- Date and time
- Subject
- Return-Path
- Received fields
- Message-ID
- SPF results
- DKIM results
- DMARC results

By analyzing these fields, it is possible to understand the path followed by an email and identify suspicious inconsistencies.

---

# 🛠️ Requirements

- Gmail or another email service
- Web browser
- Internet connection
- Mail Header Analyzer (MHA)
- WHOIS or IP lookup tool

---

# 🔬 Procedure

## Step 1: Access the Email Header

Open the email that needs to be analyzed.

For Gmail:

1. Open the email.
2. Click the **three dots (More)** menu.
3. Select **Show original**.

This displays the complete email header.


---

## Step 2: View the Original Message

After selecting **Show original**, the complete email header information will be displayed.

The email header contains metadata such as:

- Sender information
- Recipient information
- Message-ID
- Received servers
- Authentication results


---

## Step 3: Copy the Complete Email Header

Copy all the header information from the original message.

The copied header will contain information about the email's journey from the sender to the recipient.

Important fields include:

```text
From:
To:
Date:
Subject:
Return-Path:
Received:
Message-ID:
SPF:
DKIM:
DMARC:
```

---

## Step 4: Analyze the Email Header Using MHA

Paste the copied email header into the **Mail Header Analyzer (MHA)**.

The analyzer processes the header and displays important delivery and authentication information.

The email analyzed in this experiment had the subject:

```text
Fwd: Invitation to Participate in TechnoVIT 2026 – VIT Chennai
```



---

# 📬 Delivery Information

The Mail Header Analyzer displays the authentication status of the email.

The analyzed email showed:

```text
DMARC Compliant
SPF Alignment
SPF Authenticated
DKIM Alignment
DKIM Authenticated
```

These results indicate that the authentication mechanisms passed successfully.


---

# 🔄 Relay Information

The `Received` fields provide information about the route followed by the email.

The `Received` headers are analyzed to identify:

- Sending server hostname
- Sending server IP address
- Receiving server hostname
- Date and time of transmission

The experiment document explains that `Received` fields show the email path and are listed in reverse order, from the last server to the first server.



---

# 🌐 IP Address Analysis

The IP address identified during the analysis was:

```text
209.85.220.69
```

A WHOIS lookup was performed to identify the ownership of the IP address.

The result showed information related to:

```text
Organization: Google LLC
NetName: GOOGLE
NetRange: 209.85.128.0 - 209.85.255.255
```

This helps verify whether the sending infrastructure belongs to an expected organization.


---

# 🔐 SPF Analysis

SPF stands for **Sender Policy Framework**.

SPF checks whether the sender's IP address is authorized to send emails for the specified domain.

The output showed:

```text
SPF: PASS with IP 209.85.220.69
```

This indicates that the sending IP address was authorized.

---

# 🔑 DKIM Analysis

DKIM stands for **DomainKeys Identified Mail**.

DKIM helps verify that the email content has not been altered during transmission.

The output showed:

```text
DKIM: PASS with domain klu.ac.in
```

This indicates that the DKIM authentication was successfully verified.

---

# 🛡️ DMARC Analysis

DMARC uses SPF and DKIM authentication mechanisms to validate the sender.

The output showed:

```text
DMARC: PASS
```

This indicates that the email passed DMARC authentication.

---

# 📋 Original Message Analysis

The Mail Header Analyzer displayed the following information:

| Field | Value |
|---|---|
| From | Dr. R. Raja Subramanian HOD-CSE |
| Domain | klu.ac.in |
| Subject | Fwd: Invitation to Participate in TechnoVIT 2026 – VIT Chennai |
| SPF | PASS |
| DKIM | PASS |
| DMARC | PASS |
| Sending IP | 209.85.220.69 |
| IP Organization | Google LLC |



---

# 🔎 Important Fields Analyzed

## 1. From

The `From` field identifies the email address of the sender.

Example:

```text
From: Dr. R. Raja Subramanian HOD-CSE <hodcse@klu.ac.in>
```

---

## 2. To

The `To` field identifies the recipients of the email.

---

## 3. Subject

The subject of the analyzed email was:

```text
Fwd: Invitation to Participate in TechnoVIT 2026 – VIT Chennai
```

---

## 4. Received

The `Received` fields show the path followed by the email.

These fields can be used to analyze:

```text
Sending Server
Receiving Server
IP Address
Hostname
Date
Time
```

---

## 5. Message-ID

The `Message-ID` is a unique identifier assigned to an email.

The domain in the Message-ID can be compared with the sender's domain to identify possible inconsistencies.

---

# ⚠️ Spoofing Detection Checks

The following checks were performed to detect possible email spoofing:

- [x] Checked the sender's email address.
- [x] Analyzed the `Received` fields.
- [x] Identified the sending IP address.
- [x] Performed a WHOIS lookup.
- [x] Checked SPF authentication.
- [x] Checked DKIM authentication.
- [x] Checked DMARC authentication.
- [x] Compared domain information.
- [x] Checked for suspicious routing information.
- [x] Examined the Message-ID.

---

# 📊 Authentication Results

| Security Check | Result |
|---|---|
| SPF | PASS |
| DKIM | PASS |
| DMARC | PASS |
| SPF Alignment | PASS |
| DKIM Alignment | PASS |

---

# 📸 Experimental Outputs

## 1️⃣ Accessing the Email

<img width="1647" height="817" alt="1" src="https://github.com/user-attachments/assets/5cc29273-9ed7-4f50-9e9f-b3cbe1ecfef2" />
---

## 2️⃣ Viewing the Original Email Header

<img width="1171" height="636" alt="2" src="https://github.com/user-attachments/assets/de60ea70-1040-410c-ba10-84ec70cff54f" />
---

## 3️⃣ Email Header Analysis

<img width="742" height="237" alt="3" src="https://github.com/user-attachments/assets/2297d9da-d5cd-4329-b793-6d787f62f166" />
---

## 4️⃣ Authentication Results

<img width="1442" height="328" alt="4" src="https://github.com/user-attachments/assets/64b4c16e-86ab-4c0c-a1d7-3bac726e6bfa" />
---

## 5️⃣ Email Header Details

<img width="1657" height="695" alt="6" src="https://github.com/user-attachments/assets/b0bda0dc-697c-4354-90a5-c393a4446132" />
---

## 6️⃣ WHOIS IP Lookup


<img width="1438" height="770" alt="5" src="https://github.com/user-attachments/assets/4e899a3a-1f4a-4e20-ac2d-1ada0c16914a" />
---

# ✅ Result

The email header was successfully analyzed using a Mail Header Analyzer.

The following authentication results were obtained:

```text
SPF  : PASS
DKIM : PASS
DMARC: PASS
```

The sending IP address was identified as:

```text
209.85.220.69
```

A WHOIS lookup indicated that the IP address belongs to **Google LLC**.

Based on the analyzed header information and the successful SPF, DKIM, and DMARC authentication results, no obvious spoofing indication was observed in the analyzed email.

---

# 📝 Conclusion

This experiment demonstrated how email headers can be analyzed to investigate the origin and authenticity of an email.

The following information was examined:

- Email sender
- Email recipient
- Subject
- Message-ID
- Received servers
- IP address
- WHOIS information
- SPF authentication
- DKIM authentication
- DMARC authentication

The analyzed email successfully passed SPF, DKIM, and DMARC authentication.

Email header analysis is useful for detecting suspicious emails, possible spoofing attempts, phishing messages, and inconsistencies in email routing information.


Digital Forensics Lab  
Experiment No. 4
