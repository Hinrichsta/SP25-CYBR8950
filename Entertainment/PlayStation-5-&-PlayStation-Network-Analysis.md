# PlayStation 5 & PlayStation Network

## Scoring rubric
| Device Score-Category |  Rating | Reasoning | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | Hybrid | Core features work offline, but online services require an internet connection. |
| Requires Constant Connection to Company Cloud Infrastructure | Hybrid | Cloud save features, multiplayer gaming, and digital rights management rely on Sony’s infrastructure. |
| Data Storage Requirements | Hybrid | User data such as saves, media, and settings are stored both locally and in the cloud. |
| Data Gathering Risk Score | 2 | Sony gathers data including user interactions, purchase history, game telemetry, and friend activity. |
| Company Vulnerability Remediation Score | 4 | Sony has improved its security posture, launching bug bounty programs and pushing updates regularly with occasional delays and downtimes. |
| Company Vulnerability Transparency Score | 3 | Discloses major vulnerabilities and incidents. But, does not always provide full details. | 

### Total Score: 9

## Analysis  
- **Name**: PlayStation 5 & PlayStation Network (PSN)  
- **Manufacturer**: Sony Interactive Entertainment  
- **Country of Origin**: Japan-Owned Company | Manufactured in China and other regions  
- **Platform**: PlayStation Network (PSN)  

- **Internet Requirements**:  
    - Requires an internet connection for online multiplayer, cloud saves, and digital purchases [^1] 
    - PlayStation Plus subscription required for most online multiplayer games  
    - Cloud storage available for PlayStation Plus subscribers  

- **Authentication**:  
    - PlayStation accounts require a username and password [^1]
    - Two-factor authentication (2FA) is available but not mandatory  
    - Account recovery options include email and backup codes  
    - Family sharing allows multiple users to access games and subscriptions  

[^1]: [How to set up an internet connection on PlayStation consoles](https://www.playstation.com/en-us/support/connectivity/internet-connect-playstation/)

- **Data Transmission Security**: [^2]  
    - Uses TLS/SSL encryption for account and transaction security  
    - Network communication is encrypted to protect user data and prevent unauthorized access
 
[^2]: [Online Safety, Account Security, and Privacy](https://www.playstation.com/en-us/privacy-security-safety/)

- **Physical Security**:   
    - Hardware-based Trusted Platform Module (TPM) ensures integrity checks  
    - Physical USB and disc drive access are limited by system permissions [^3]
 
[^3]: [USB drive on PS5 & PS4 Consoles](http://playstation.com/en-us/support/hardware/play-video-music-discs-usb-drives/#:~:text=How%20to%20play%20video%20from,exFAT%20or%20FAT32%20file%20system.&text=Using%20a%20computer%2C%20create%20a,video%20files%20in%20the%20folder.) 

- **Storage**:  
    - Cloud storage available for PlayStation Plus members for game saves  
    - Internal SSD for fast game loading and storage encryption  
    - External USB storage supported for additional game storage [^3]

- **Data Requirements**:  
    - Online gaming requires a stable internet connection [^1] (minimum 5 Mbps, recommended 15-25 Mbps for high-performance gaming)  

- **Data Gathering**:  
    - Collects user gameplay activity, interactions, purchases, and communication logs  
    - Data is used for personalized recommendations, marketing, and service improvements  
    - Privacy settings allow users to limit data collection and sharing  [^2]  

- **Vulnerability Remediation**:  
    - Regular system updates and patches to address security vulnerabilities  
    - Security team monitors and responds to emerging threats  
    - Bug bounty program through [HackerOne](https://hackerone.com/playstation) for vulnerability reporting [^4] [^5]

[^4]: [hacker-one-sony](https://hackerone.com/sony)
[^5]: [hacker-one-playstation](https://hackerone.com/playstation)

- **Vulnerability Transparency**:  
    - Discloses security updates via official PlayStation blog and support pages  
    - **Past breaches and vulnerabilities**:  
        - **2011 PlayStation Network breach** – Exposed data of 77 million users, leading to major security overhauls  
        - **2022 PlayStation 4 & 5 exFAT vulnerability (CVE-2022-3349)** – Heap-based buffer overflow risk  
        - **2024 PlayStation WebKit vulnerability** – Affected both PlayStation 4 and 5, allowing potential code execution
