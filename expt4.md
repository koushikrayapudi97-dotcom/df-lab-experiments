# Experiment No. 4: Analyze Email Headers and Detect Email Spoofing Using MHA

## Aim

To analyze an email header using Mail Header Analyzer (MHA) and detect possible email spoofing by examining email routing information and authentication results.

## Requirements

* Gmail / Outlook / Yahoo Mail
* Mail Header Analyzer (MHA)
* Web browser
* WHOIS / IP lookup tool
* Internet connection

## Procedure

### Step 1: Access the Email Header

**Gmail:**

1. Open the email.
2. Click the three-dot menu in the upper-right corner.
3. Select **Show original**.

**Outlook:**

1. Open the email.
2. Click **File**.
3. Select **Properties**.
4. Locate the **Internet headers** section.

**Yahoo:**

1. Open the email.
2. Click the three-dot menu.
3. Select **View raw message**.

### Step 2: Copy the Email Header

Copy the complete email header displayed by the email service.

### Step 3: Analyze the Header Using MHA

1. Open Mail Header Analyzer.
2. Paste the copied email header into the analyzer.
3. Submit the header for analysis.
4. Examine the parsed header information.
5. Identify the `From`, `To`, `Return-Path`, `Received`, and `Message-ID` fields.
6. Check the SPF, DKIM, and DMARC authentication results.

### Step 4: Analyze the Received Fields

Examine the `Received` fields to determine:

* Sending server hostname
* Sending server IP address
* Receiving server
* Date and time of transmission
* Sequence of mail servers

The `Received` headers should be analyzed from the **bottom upward** to trace the email's path.

### Step 5: Check IP Addresses and Hostnames

Use an IP lookup or WHOIS tool to check the IP addresses found in the `Received` headers.

Verify whether:

* The IP belongs to the expected mail server.
* The hostname matches the IP address.
* The sending server appears legitimate.
* Any unexpected server or IP address is present.

### Step 6: Check SPF, DKIM, and DMARC

Record the authentication results.

| Check | Result    | Observation                                |
| ----- | --------- | ------------------------------------------ |
| SPF   | PASS/FAIL | Check whether the sending IP is authorized |
| DKIM  | PASS/FAIL | Check whether the DKIM signature is valid  |
| DMARC | PASS/FAIL | Check domain authentication and alignment  |

### Step 7: Analyze Message-ID

Check the domain used in the `Message-ID` and compare it with the sender's domain.

### Step 8: Identify Possible Spoofing Indicators

Check for:

* `From` and `Return-Path` domain mismatch
* Suspicious IP addresses
* Unexpected hostnames
* SPF failure
* DKIM failure
* DMARC failure
* Unusual timestamps
* Inconsistent mail-server routing
* Suspicious Message-ID domain

## Sample Header

```text
Received: from mail.example.com (mail.example.com [192.0.2.1])
  by mail.receiver.com with ESMTP id u29si8604336pjs.40.2023.08.10.07.00.16;
  Thu, 10 Aug 2023 07:00:16 -0700 (PDT)

Received: by mail.example.com with SMTP id a1mr1243772ywh.51;
  Thu, 10 Aug 2023 07:00:15 -0700 (PDT)

Message-ID: <CA+7eu=4pSeXgQ@mail.example.com>
```

## Analysis

* The email passed through `mail.example.com` before reaching `mail.receiver.com`.
* The sending IP address shown is `192.0.2.1`.
* The timestamps in the `Received` fields are in logical chronological order.
* The `Message-ID` contains the `mail.example.com` domain.
* SPF, DKIM, and DMARC results should be checked in the actual email header.
* Any authentication failure combined with domain or IP inconsistencies should be investigated as a possible spoofing attempt.

## Observation

The email header was successfully parsed using MHA. The sender information, mail-server path, IP address, Message-ID, and email authentication results were examined for inconsistencies.

## Result

The email header was successfully analyzed using Mail Header Analyzer, and possible email spoofing indicators were identified by examining the **Received, Return-Path, Message-ID, SPF, DKIM, and DMARC** fields.

## Conclusion

Email header analysis using MHA can be used to trace the email's delivery path and identify inconsistencies that may indicate email spoofing or phishing.
<img width="1918" height="917" alt="Screenshot 2026-08-23 220503" src="https://github.com/user-attachments/assets/f6168e70-7950-41cf-a3d4-e94a847a854a" />
<img width="1920" height="1080" alt="Screenshot 2026-08-23 220859" src="https://github.com/user-attachments/assets/4ca53dbc-cb04-45af-812f-6323d44e5d88" />
<img width="1920" height="1080" alt="Screenshot 2026-08-23 221240" src="https://github.com/user-attachments/assets/a17b9940-d4d7-495b-a00b-5d57dadccabc" />
<img width="1920" height="1080" alt="Screenshot 2026-08-23 221255" src="https://github.com/user-attachments/assets/d1fad2db-0c0c-4274-a789-c32867c66c4d" />
<img width="1920" height="1080" alt="Screenshot 2026-08-23 221305" src="https://github.com/user-attachments/assets/a102d400-2f1d-40c3-9739-bfc01200f5a8" />
<img width="1920" height="1080" alt="Screenshot 2026-08-23 221319" src="https://github.com/user-attachments/assets/7cad7740-4f0a-4e4d-9658-6d728ffe11f4" />
<img width="1920" height="1080" alt="Screenshot 2026-08-23 221327" src="https://github.com/user-attachments/assets/f251acc0-a62f-420a-bc48-0acbe7a0be8a" />
<img width="1920" height="1080" alt="Screenshot 2026-08-23 221339" src="https://github.com/user-attachments/assets/5fba610d-919f-48d9-8cec-afbb4a488f31" />








