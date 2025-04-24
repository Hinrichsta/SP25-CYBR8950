# VTech Toys

## Scoring rubric
| Device Score-Category |  Rating | Reasoning | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | Hybrid | Core features work offline, but online services require an internet connection. |
| Requires Constant Connection to Company Cloud Infrastructure | Yes | Some features require connection to Sony’s cloud, but offline play is possible. |
| Data Storage Requirements | Cloud | Uses both local storage and cloud storage for different types of data. |
| Data Gathering Risk Score | 1 | Collects significant user data, including purchases, interactions, and gameplay activity. |
| Company Vulnerability Remediation Score | 3 | Regular updates and a bug bounty program exist, but some patches are delayed. |
| Company Vulnerability Transparency Score | 2 | Discloses major vulnerabilities but does not always provide full details. | 

### Total Score: 6/15

## Analysis  
- **Name**: VTech Connected Toys & VTech Cloud
- **Manufacturer**: VTech Holdings Limited
- **Country of Origin**: Hong Kong-based company | Products manufactured in China and other regions
- **Platform**: VTech Cloud, Learning Lodge, Kid Connect​

- **Internet Requirements**:  
    - Internet connectivity is required for downloading apps, games, and e-books via Learning Lodge.
    - Kid Connect enables messaging between children and approved contacts, necessitating an internet connection.
    - Software updates and content downloads are facilitated through an internet connection

- **Authentication**:  
    - User accounts require a username and password.
    - Two-factor authentication (2FA) is not currently supported.
    - Account recovery options include security questions and email verification.
    - Parental controls allow parents to manage and monitor their child's account and interactions.

- **Data Transmission Security**:  
    - Post-2015, VTech implemented HTTPS encryption for data transmission.
    - Prior to the 2015 breach, data was transmitted without proper encryption, exposing sensitive information.​

- **Physical Security**:  
    - Devices lack advanced physical security measures such as secure boot processes or hardware-based Trusted Platform Modules (TPMs).
    - Physical access to devices is not restricted beyond standard user permissions.

- **Storage**:  
    - User data, including personal information and activity logs, is stored on VTech's cloud platform.
    - Devices have limited internal storage for apps and user data.
    - External storage options are minimal and primarily used for media files.
      - Encryption of stored data has been improved following the 2015 breach.

- **Data Requirements**:  
    - Stable internet connection required for downloading content and using interactive features.
    - Data usage varies depending on the content downloaded and frequency of use.

- **Data Gathering**:  
    - Collects personal information including names, birthdates, and photos of children and parents.
    - Activity logs, chat messages, and usage data are collected through services like Kid Connect.
    - Data is used for service improvement and personalized content delivery.
    - Privacy settings allow parents to manage data collection and sharing preferences.

- **Vulnerability Remediation**:  
    - Regular software updates are provided to address security vulnerabilities.
    - Post-2015, VTech has overhauled its data security practices to comply with COPPA regulations.
    - Employee training and improved security protocols have been implemented to prevent future breaches.
      
- **Vulnerability Transparency**:  
    - Security updates and privacy policy changes are communicated through official VTech channels.
    - Following the 2015 breach, VTech settled with the FTC, agreeing to enhance data security measures and pay a $650,000 fine.
 
    - **Past breaches and vulnerabilities**:  
        - **2015 VTech Data Breach** –  WPA2 vulnerability in 1st-gen Echo devices
          - A hacker accessed VTech's servers, compromising data of approximately 6.4 million children and 4.9 million parents.
          - Stolen data included names, email addresses, passwords, security questions, children's birthdates, photos, and chat logs.
          - The breach was due to outdated encryption practices and lack of basic security measures like HTTPS.
        
