# Beko Smart Fridge

## Scoring rubric
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | Hybrid | Device operates offline, but remote features require cloud.[^1] |
| Requires Constant Connection to Company Cloud Infrastructure | Hybrid | Cloud not needed for basic operation, but many smart features depend on HomeWhiz.[^1] |
| Data Storage Requirements | Hybrid | Some settings stored locally, usage data stored in HomeWhiz cloud.[^3] |
| Data Gathering Risk Score | 4 | Limited telemetry collected and used only for functionality.[^2] |
| Company Vulnerability Remediation Score | 4 | Coordinated disclosure process, IASME-certified, but no bug bounty.[^4] [^5] |
| Company Vulnerability Transparency Score | 4 | No public CVEs, but third-party certification and clear disclosure policy.[^4] [^5] | 

### Total Score: 12

## Analysis
- **Name**:Beko Smart Fridge 
- **Manufacturer**: Beko US - Parent Company: Arçelik A.Ş.
- **Country of Origin**: Turkey
- **Platform**: HomeWiz IoT Ecosystem
- **Internet Requirements**:
    - Not required to utilize device, but remote control features are unavailable if not connected.[^1] [^2]
- **Authentication**
    - User authentication is required to access HomeWiz App, MFA not enforced by default.[^3]
    - Requires Wi-Fi credentials during setup and stores information like temperature logs, usage stats, and connected account info.[^1]
- **Data Transmission Security**
    - HomeWiz has a IASME IoT Security Assured certification, and this confirms they use encrypted communication protocols HTTPS/TLS for cloud interactions and data transmissions between the device and app.
- **Physical Security**
    - Standard appliance security with screws and accessible parts. Could lead to tampering or data theft with physical access.
- **Storage**
    - Operates with hybrid storage because it stores device settings locally, but cloud-connected features like usage logs, app preferences, notifications are stored on HomeWhiz servers.[^3]
- **Data Requirements**
    - No specific bandwidth requirements disclosed, but expected to function on a 2.4GHz Wi-Fi network with standard home broadband.[^1]
- **Data Gathering**
  - Collects telemetry for things like performance diagnostics, opening/closing doors, and energy consumption data. Data is reportedly only used for app-based functionality and user notifications.[^2]
- **Vulnerability Remediation**
  - Beko's parent company Arçelik has implemented structured vulnerability remediation processes and reporting tools. They operate a policy of coordinated disclosure for dealing with reports of security vulnerabilities and issues.
- **Vulnerability Transparency**
  - There are no publicly disclosed CVEs identified for Beko smart fridges as of the writing of this research. However, Arçelik's participation in third-party audits and participation in IASME certification shows they have a proactive approach to transparency, even if individual disclosures are not posted on public registries like the National Vulnerability Database.[^4] [^5]
  - No Bug bounty program available, but they do take reports of vulnerabilities. [^5]

[^1]: [HomeWhiz Setup](https://documents.beko.com/WM/7178571300/en-GB/126007307153201419.html)
[^2]: [Smart Home Integration with Beko Appliances](https://www.beko.com/gulf/ae-en/Blog/tips-and-tricks/smart-home-integration-with-beko-appliances)
[^3]: [A secure connected home](https://www.homewhiz.com/security/)
[^4]: [One smart Beko fridge](https://iasme.co.uk/blog/one-smart-beko-fridge-and-its-journey-to-become-iot-security-assured-a-case-study-with-arcelik/)
[^5]: [Vulnerability Disclosure Procedure](https://www.bekoplc.com/vulnerability-disclosure-procedure/)
