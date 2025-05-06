# Amazon Alexa & Echo Devices

## Scoring rubric
| Device Score-Category |  Rating | Reasoning | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | Yes | Alexa’s primary functions depend heavily on internet access. While some limited offline functionality (like local alarms) exists, the device is essentially non-functional without a connection. |
| Requires Constant Connection to Company Cloud Infrastructure | Yes | Voice queries are processed in Amazon’s cloud. Features such as shopping lists, reminders, and most smart home commands route through AWS infrastructure, confirming constant cloud reliance. |
| Data Storage Requirements | Hybrid | Voice data, settings, and user interactions are stored in the cloud, but some basic preferences may be cached locally on the device. |
| Data Gathering Risk Score | 1 | Alexa devices are well-known for collecting extensive user data: voice recordings, smart home usage, third-party integrations, and purchasing history. |
| Company Vulnerability Remediation Score | 4 | Amazon maintains a vulnerability disclosure program and provides frequent security updates. |
| Company Vulnerability Transparency Score | 3 | Amazon discloses high-profile vulnerabilities, but sometimes lacks in spreading of information to consumers. | 

### Total Score: 8

## Analysis  
- **Name**: Amazon Alexa & Echo Devices
- **Manufacturer**: Aamazon
- **Country of Origin**: U.S.-Based Company | Devices Manufactured in China and other regions
- **Platform**: Alexa Voice Services (AVS)

- **Internet Requirements**:  
    - Requires an internet connection for voice processing, cloud services, and smart home integration [^1]
    - Amazon account required for full device functionality and personalized services
    - Cloud services include voice recognition, user preferences, and smart device management
[^1]: [Aamazon Device Requirements](https://developer.amazon.com/en-US/docs/alexa/smarthome/wwa-device-requirements.html)

- **Authentication**:  
    - Amazon accounts require an email address and password
    - Two-factor authentication (2FA) available and encouraged, especially after past breaches [^2]
    - Account recovery includes email/phone verification and password reset options
[^2]: [Multi-Factor Authentication](https://www.amazon.com/gp/help/customer/display.html?nodeId=G9MX9LXNWXFKMJYU)

- **Data Transmission Security**:  
    - Uses HTTPS and TLS encryption for voice data and cloud communication [^3]
    - Voice recordings are encrypted and stored on Amazon’s cloud infrastructure [^4]
    - Past vulnerabilities involved potential voice injection and improper access controls

[^3]: [Developer WWA-Security](https://developer.amazon.com/en-US/docs/alexa/smarthome/wwa-security.html)
[^4]: [Alexa Privacy Hub](https://www.amazon.com/Alexa-Privacy-Hub/b?ie=UTF8&node=19149155011)

- **Physical Security**:  
    - No TPM in most Alexa devices; secure boot mechanisms implemented in newer models
    - Echo devices are not hardened against physical tampering (such as dolphin attacks) [^5]
    - Microphone mute button is physical, offering a hardware-level disconnect

[^5]: [Dolphin Attacks 3.2](https://www.sciencedirect.com/science/article/pii/S2667295222000393#:~:text=3.2.&text=These%20vulnerabilities%20can%20be%20exploited,avenue%20for%20attacking%20%5B11%5D.)

- **Storage**:  
    - Voice recordings and interaction logs stored in Amazon’s cloud (when voice-activated) [^6] 
    - No end-user control over encryption of stored voice data
    - Local device storage used for minimal caching and temporary data

[^6]: [Alexa, Echo Devices, and Your Privacy](https://www.amazon.com/gp/help/customer/display.html?nodeId=GVP69FUJ48X9DK8V)

- **Data Requirements**:
    - Continuous internet connection required for real-time processing
    - Firmware updates delivered periodically and installed upon request ("check for software updates")

- **Data Gathering**:  [^6]     
    - Collects voice recordings, device interactions, smart home activity, and usage patterns
    - Data used for improving AI, personalization, and targeted advertising
    - Privacy settings allow deletion of voice history and management of permissions, though defaults favor data retention

- **Vulnerability Remediation**:  
    - Regular firmware and cloud-side updates address vulnerabilities and performance
    - Amazon Vulnerability Research Program (VRP) offers structured disclosure channels [^7]
    - Actively engages with security researchers and issues timely patches

[^7]: [Amazon Vulnerability Research Program](https://hackerone.com/amazonvrp?type=team)
 
- **Vulnerability Transparency**:  
    - Major vulnerabilities disclosed via Amazon's security bulletins and coordinated disclosures
    - **Past breaches and vulnerabilities**:  
        - **2017 – KRACK Wi-Fi Attack (CVE-2017-13077 & CVE-2017-13078)** –  WPA2 vulnerability in 1st-gen Echo devices
        - **2018 – Alexa Skill Eavesdropping (CVE-2018-11567)** – Malicious skills could secretly record users
        - **2020 – Echo Show RCE (ZDI-20-537)** - Integer overflow allowed remote code execution via malicious pages
        - **2022 – "Alexa vs. Alexa" Attack (CVE-2022-25809)** - Self-triggered voice commands via malicious Bluetooth or skills
        - **2023 – Near-Ultrasound Command Injection (CVE-2023-33248)** – Inaudible frequency voice injection on Echo Dot 2nd/3rd gen
        - **2020 – Alexa Web Service Exploitation** – Allowed attackers to access voice history via crafted links
