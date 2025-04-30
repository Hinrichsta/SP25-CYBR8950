# VTech Connected Toys & VTech Cloud

## Scoring rubric
| Device Score-Category |  Rating | Reasoning | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | Hybrid | Core features work offline, but online services require an internet connection. |
| Requires Constant Connection to Company Cloud Infrastructure | Yes | Some features require connection to Sony’s cloud, but offline play is possible. |
| Data Storage Requirements | Cloud | Uses both local storage and cloud storage for different types of data. |
| Data Gathering Risk Score | 2 | Collects significant user data, including purchases, interactions, and gameplay activity. |
| Company Vulnerability Remediation Score | 4 | Regular updates and a bug bounty program exist, but some patches are delayed. |
| Company Vulnerability Transparency Score | 3 | Discloses major vulnerabilities but does not always provide full details. | 

### Total Score: 11/15

## Analysis  
- **Name**: VTech Connected Toys & VTech Cloud
- **Manufacturer**: VTech Holdings Limited
- **Country of Origin**: Hong Kong-based company | Products manufactured in China and other regions 
- **Platform**: VTech Cloud, Learning Lodge, Kid Connect​

- **Internet Requirements**:  
    - Internet connectivity is required for downloading apps, games, and e-books via Learning Lodge.
    - Kid Connect enables messaging between children and approved contacts, necessitating an internet connection. 

- **Authentication**:  
    - VTech Kid Connect requires a valid email address and requires an account to be set up with a password. 
    - Parent user is required to create accounts for child accounts, which are restricted otherwise. [^1]

 [^1]: [Creating an Account and Registering on Learning Lodge](https://www.vtechkids.com/tutorials/innotab3)

- **Data Transmission Security**:  
    - VTech transmits data over a secure HTTPS connection using TLS technology [^2]
    - Prior to the 2015 breach, data was transmitted without proper encryption, exposing sensitive information.​

[^2]: [VTech Privacy Policy](https://www.vtechda.com/legal/version/view.aspx?country=US&lang=eng&x=4&y=1)

- **Physical Security**:  
    - VTech does not explicitly mention secure boot processes or hardware-based Trusted Platform Modules (TPMs) for their devices
    - Physical access to devices is not restricted beyond standard user permissions.

- **Storage**:  
    - User data, including personal information and activity logs, and imge of face and body features is stored on VTech's servers. [^2]
    - Devices have limited internal storage for apps and user data.

- **Data Requirements**:  
    - Internet connection is required to download content and use interactive features of Learning Lodge & Kid Connect. [^3]

[^3]: [Introduction to and Installing Learning Lodge](https://www.vtechkids.com/tutorials/innotab3)

- **Data Gathering**:  
    - Collects personal information, including names, birthdates, and photos of users' face and body features. [^2]
    - Activity logs, chat messages, and usage data are collected through services like Kid Connect. [^2]

- **Remediation & Disclosure**:  
    - Regular software updates are provided to address security vulnerabilities.
    - VTech follows COPPA regulations. 
      
- **Company Transparency**:  
    - Security updates and privacy policy changes are communicated through official VTech channels.
    - VTech settled with the FTC, agreeing to enhance data security measures and pay a $650,000 fine after violating children's privacy laws. [^4]
 
    - **Past breaches and vulnerabilities**:  
        - **2015 VTech Data Breach** –  WPA2 vulnerability in 1st-gen Echo devices
          - A hacker accessed VTech's servers in 2015 and was able to harvest sensitive user data as it was NOT encrypted, even though their privacy policy at the time stated it did in fact encrypt data. [^4]
          - Stolen data included names, email addresses, passwords, security questions, children's birthdates, photos, and chat logs.
         
[^4]: [Electronic Toy Maker VTech Settles FTC Allegations That it Violated Children’s Privacy Law and the FTC Act](https://www.ftc.gov/news-events/news/press-releases/2018/01/electronic-toy-maker-vtech-settles-ftc-allegations-it-violated-childrens-privacy-law-ftc-act)
        
