# Roku Television

## Scoring rubric
| Device Score-Category |  Rating | Reasoning | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | x | Core features work offline, but online services require an internet connection. |
| Requires Constant Connection to Company Cloud Infrastructure | x | Some features require connection to Sony’s cloud, but offline play is possible. |
| Data Storage Requirements | x | Uses both local storage and cloud storage for different types of data. |
| Data Gathering Risk Score | x | Collects significant user data, including purchases, interactions, and gameplay activity. |
| Company Vulnerability Remediation Score | x | Regular updates and a bug bounty program exist, but some patches are delayed. |
| Company Vulnerability Transparency Score | x | Discloses major vulnerabilities but does not always provide full details. | 

### Total Score: x/15

## Analysis  
- **Name**: Roku Television & Roku Platform
- **Manufacturer**: Roku, Inc.
- **Country of Origin**: U.S.-Based Company | Devices Manufactured in China and other regions
- **Platform**: Roku OS & The Roku Channel

- **Internet Requirements**:  
    - Requires an internet connection for streaming services, app updates, and cloud-based features
    - Roku account required for full device functionality and personalization 
    - Cloud services include content syncing, device preferences, and advertising personalization

- **Authentication**:  
    - Roku accounts require an email address and password
    - Two-factor authentication (2FA) is supported but only enforced during incidents 
    - Account recovery includes email verification and password reset options

- **Data Transmission Security**:  
    - Utilizes HTTPS and TLS encryption for data transmission
    - Cloud communication and app traffic are secured, but may depend on third-party integrations
    - Vulnerabilities have existed in local network control APIs

- **Physical Security**:  
    - No TPM or secure boot mechanisms publicly disclosed for most Roku devices
    - Devices are designed for open accessibility, not hardened against physical tampering
    - USB ports and HDMI interfaces do not offer encryption or access restriction features

- **Storage**:  
    - Cloud storage used for account preferences, watch history, and system settings
    - Devices typically use internal flash storage for app data and caching
    - No end-user encryption control over local or cloud-stored data

- **Data Requirements**:  
    - Stable internet connection required (minimum 3 Mbps for SD, 25 Mbps for 4K UHD)  
    - Firmware and channel updates delivered periodically, typically under 500 MB
    - Usage and ad tracking data synced regularly with Roku cloud services

- **Data Gathering**:  
    - Collects viewing history, app usage, ad interactions, device identifiers, and location approximation
    - Data used for targeted advertising, personalization, analytics, and third-party sharing
    - Privacy settings available but can be complex to fully disable tracking 

- **Vulnerability Remediation**:  
    - Regular software updates addressing performance and security flaws  
    - Monitored disclosures through coordinated vulnerability disclosures and independent research
    - No formal bug bounty program publicly disclosed 

- **Vulnerability Transparency**:  
    - Security fixes typically released silently or noted in general update logs
    - **Past breaches and vulnerabilities**:  
        - **2018 – Roku Remote API Exploit (CVE-2018-11314)** – Allowed attackers on the local network to spoof remote commands. Patched in firmware.
        - **2022 – Realtek SDK Flaw (CVE-2022-27152)** – Arbitrary file modification vulnerability due to Realtek SDK used in Roku devices. Patched in newer firmware.
        - **2023 – Roku Indoor Camera SE**
           - (CVE-2023-6322) – Buffer overflow in message parsing
           - (CVE-2023-6324) – DTLS hash-based hijack enabling command access
        - **2024 - Credential Stuffing Incidents** - Over 500,000 Roku accounts compromised due to reused passwords from unrelated breaches. Roku enforced 2FA and reset passwords.
