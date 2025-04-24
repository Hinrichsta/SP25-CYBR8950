## Scoring rubric
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection |  |  |
| Requires Constant Connection to Company Cloud Infrastructure |  |  |
| Data Storage Requirements |  |  |
| Data Gathering Risk Score |  |  |
| Company Vulnerability Remediation Score |  |  |
| Company Vulnerability Transparency Score |  |  | 

### Total Score: 

# Beko Smart Fridge
## Analysis
- **Name**:Beko Smart Fridge 
- **Manufacturer**: Beko US - Parent Company: Arçelik A.Ş.
- **Country of Origin**: Turkey
- **Platform**: HomeWiz IoT Ecosystem
- **Internet Requirements**:
    - Not required to utilize device, but remote control features are unavailable if not connected.[^1] [^2]
[^1]: [HomeWhiz Setup](https://documents.beko.com/WM/7178571300/en-GB/126007307153201419.html)
[^2]: [Smart Home Integration with Beko Appliances](https://www.beko.com/gulf/ae-en/Blog/tips-and-tricks/smart-home-integration-with-beko-appliances)
- **Authentication**
    - User authentication is required to access HomeWiz App, MFA not enforced by default.[^3]
    - Requires Wi-Fi credentials during setup and stores information like temperature logs, usage stats, and connected account info.[^1]
[^3]: [A secure connected home](https://www.homewhiz.com/security/)
- **Data Transmission Security**
    - HomeWiz has a IASME IoT Security Assured certification, and this confirms they use encrypted communication protocols HTTPS/TLS for cloud interactions and data transmissions between the device and app.
- **Physical Security**
    - Standard appliance security with screws and accessible parts. Could lead to tampering or data theft with physical access.
- **Storage**
    - Operates with hybrid storage because it stores device settings locally, but cloud-connected features like usage logs, app preferences, notifications are stored on HomeWhiz servers.
- **Data Requirements**
    - No specific bandwidth requirements disclosed, but expected to function on a 2.4GHz Wi-Fi network with standard home broadband.
- **Data Gathering**
  - Collects telemetry for things like performance diagnostics, opening/closing doors, and energy consumption data. Data is reportedly only used for app-based functionality and user notifications.
- **Vulnerability Remediation**
  - Beko's parent company Arçelik has implemented structured vulnerability remediation processes and reporting tools. They operate a policy of coordinated disclosure for dealing with reports of security vulnerabilities and issues.
- **Vulnerability Transparency**
  - There are no publicly disclosed CVEs identified for Beko smart fridges as of the writing of this research. However, Arçelik's participation in third-party audits and participation in IASME certification shows they have a proactive approach to transparency, even if individual disclosures are not posted on public registries like the National Vulnerability Database.
  - No Bug bounty program available, but they do take reports of vulnerabilities. 

## Scoring rubric
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection |  |  |
| Requires Constant Connection to Company Cloud Infrastructure |  |  |
| Data Storage Requirements |  |  |
| Data Gathering Risk Score |  |  |
| Company Vulnerability Remediation Score |  |  |
| Company Vulnerability Transparency Score |  |  | 

### Total Score: 

#### Citations
https://www.bekoplc.com/vulnerability-disclosure-procedure/
https://www.homewhiz.com/security/
https://www.beko.com/gulf/ae-en/Blog/tips-and-tricks/smart-home-integration-with-beko-appliances
https://documents.beko.com/WM/7178571300/en-GB/126007307153201419.html
https://iasme.co.uk/blog/one-smart-beko-fridge-and-its-journey-to-become-iot-security-assured-a-case-study-with-arcelik/



