# AEG Smart Oven

## Scoring rubric
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | Hybrid | The oven functions offline, but smart features like remote control and updates require internet.[^1] |
| Requires Constant Connection to Company Cloud Infrastructure | Hybrid | 	Cloud enhances user functionality and features, but is not needed for core cooking functions.[^1] |
| Data Storage Requirements | Hybrid | 	Core functionality is local and cloud is used for user preferences,monitoring, and diagnostics.[^1][^7] |
| Data Gathering Risk Score | 4 | Limited collection includes usage patterns, temperature but claims it is for performance and app use.  No sensitive data shared. [^2][^3][^7] |
| Company Vulnerability Remediation Score | 3 | 	Electrolux provides regular firmware updates and has documented update practices but no public bug bounty program. [^1][^7]  |
| Company Vulnerability Transparency Score | 3 | Provides privacy documentation, but lacks a dedicated vulnerability disclosure portal or CVE list.[^2][^3][^4] | 

### Total Score: 10

## Analysis
- **Name**: AEG Smart Oven
- **Manufacturer**: AEG - Parent Company: Electrolux Group
- **Country of Origin**: Sweden
- **Platform**: AEG App (Electrolux platform)
- **Internet Requirements**:
  - Not required to utilize device, but remote control, remote monitoring, software updates, and integration with voice assistants features are unavailable if not connected.[^1][^8]
- **Authentication**
  - User authentication is required to access AEG App, MFA not enforced by default.[^1][^8]
- **Data Transmission Security**
  - AEG Connected App uses encrypted communication protocols HTTPS/TLS for cloud interactions and data transmissions between the device and app.[^1] [^7]
- **Physical Security**
  - Standard appliance security with screws and accessible parts. Could lead to tampering or data theft with physical access.
- **Storage**
  - The ovens store essential operational data locally. Usage statistics, preferences, and diagnostics are stored in the cloud via the AEG Connected platform.[^3] [^7]
- **Data Requirements**
  -  No specific bandwidth requirements are disclosed. The oven connects via 2.4GHz Wi-Fi, suitable for standard home broadband connections.[^8]
- **Data Gathering**
  - The ovens collect data such as usage patterns, temperature settings, and diagnostic information to enhance user experience and for maintenance purposes.[^2], [^3], [^7]
- **Vulnerability Remediation**
  - Electrolux has established processes for vulnerability remediation, including regular software updates and patches delivered through the AEG Connected App.[^1] [^7]
- **Vulnerability Transparency**
  - There are no publicly disclosed CVEs specific to AEG smart ovens. Electrolux provides a privacy policy outlining data handling practices but lacks a dedicated vulnerability disclosure program.[^2] [^4][^6]
 
[^1]: [AEG Redefine smart living](https://apps.apple.com/ie/app/aeg/id1599494494?)
[^2]: [PROTECTION OF YOUR PERSONAL DATA](https://www.electroluxgroup.com/privacy/en/)
[^3]: [Collection Statement](https://www.electrolux.com.au/privacy/)
[^4]: [PRIVACY POLICY](https://www.electroluxprofessional.com/au/data-privacy-statement/)
[^5]: [AEG Built-in Electric Single Oven](https://www.harveynorman.ie/home-appliances/cooking-appliances/ovens/single-ovens/aeg-built-in-electric-single-oven-bpe948730m.html?)
[^6]: [Smart ovens do really dumb stuff to check for Wi-Fi](https://www.theregister.com/2023/01/26/smart_ovens_do_dumb_stuff/?)
[^7]: [Electrolux Australia Privacy Policy](https://shop.aegaustralia.com.au/privacy-policy/?)
[^8]: [How to connect your AEG oven to the app](https://support.aeg.co.uk/support-articles/article/how-to-connect-your-aeg-oven-to-the-app?srsltid=AfmBOoo51VIrCwyCxVGC4U8XCghLNxq80ch3WJxCZkJZQzaRpHsqez2w&locale=en-GB)
