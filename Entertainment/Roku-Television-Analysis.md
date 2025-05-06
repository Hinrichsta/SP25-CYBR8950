# Roku Television

## Scoring rubric
| Device Score-Category |  Rating | Reasoning | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | Hybrid | Some play features work offline, but connectivity is needed for downloading new content or syncing to the VTech cloud. |
| Requires Constant Connection to Company Cloud Infrastructure | Yes | VTech devices are heavily dependent on their cloud services for content, learning apps, and user accounts. |
| Data Storage Requirements | Cloud | VTech stores most user data in the cloud, including personal info and chat logs. |
| Data Gathering Risk Score | 1 | Child and parent data gathered includes voice recordings, names, locations, and usage behavior. |
| Company Vulnerability Remediation Score | 3 | They responded to past breaches by improving security, but lack a formal bug bounty program and rely on reactive, not proactive, security. |
| Company Vulnerability Transparency Score | 2 | Post-incident disclosures have been vague. Outside of major incidents. | 

### Total Score: 6

## Analysis  
- **Name**: Roku Television & Roku Platform
- **Manufacturer**: Roku, Inc.
- **Country of Origin**: U.S.-Based Company | Devices Manufactured in China and other regions
- **Platform**: Roku OS & The Roku Channel

- **Internet Requirements**:  
    - Requires an internet connection for streaming services, app updates, and cloud-based features [^1]
    - Roku account required for full device functionality and personalization 
    - Cloud services include content syncing, device preferences, and advertising personalization

[^1]: [Connect your Roku streaming device to the internet](https://support.roku.com/article/115015760328)

- **Authentication**:  
    - Roku accounts require an email address and password [^2]
    - Two-factor authentication (2FA) is required [^2]
 
[^2]: [How to use two-step verification to sign in to your Roku account](https://support.roku.com/article/22482363662103)

- **Data Transmission Security**:  
    - Utilizes HTTPS and TLS encryption for data transmission [^3]
    - Cloud communication and app traffic are secured, but may depend on third-party integrations
  
[^3]: [Roku Data Processing Terms](https://docs.roku.com/published/dataprocessingterms/en/gb)

- **Physical Security**:  
    - Roku platform has been designed to be hardened against unauthorized attack [^4]
    - Roku OS also supports HDCP for content copy protection between the Roku player's HDMI port [^7]

[^4]: [Security on the Roku platform](https://developer.roku.com/docs/features/security.md)
[^7]: [DRM & content protection](https://developer.roku.com/docs/specs/media/content-protection.md)

- **Storage**:  
    - Cloud storage used for account preferences, watch history, and system settings
    - Roku devices have small storage spaces as they do not contain the streamed content, but rather host it

- **Data Requirements**:  
    - Stable internet connection required [^1]
    - Firmware and channel updates are delivered periodically, typically under 500 MB

- **Data Gathering**:  
    - Collects viewing history, app usage, ad interactions, device identifiers, and location approximation [^5]
    - Data used for targeted advertising, personalization, analytics, and third-party sharing [^6]

[^5]: [Roku Data Processing Terms](https://docs.roku.com/published/dataprocessingterms/en/gb)
[^6]: [Privacy Policy](https://docs.roku.com/published/userprivacypolicy)

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
