# LG Smart Oven

## Scoring rubric
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | Hybrid | Basic functions operate offline; advanced features require internet connectivity.[^1] |
| Requires Constant Connection to Company Cloud Infrastructure | Hybrid | Core functions are local; cloud connection needed for remote features.[^1] |
| Data Storage Requirements | Hybrid | Operational data stored locally. Usage stats and preferences stored in the cloud.[^3][^8] |
| Data Gathering Risk Score | 3 | Moderate data collection, including usage patterns and diagnostics.[^3] |
| Company Vulnerability Remediation Score | 4 | Known vulnerabilities have been addressed with patches and proactive measures are in place.[^5] |
| Company Vulnerability Transparency Score | 3 | Security bulletins are published, but appliance-specific disclosures are less frequent.[^5] | 

### Total Score: 10

## Analysis
- **Name**: LG Smart Oven
- **Manufacturer**: LG Electronics
- **Country of Origin**: South Korea
- **Platform**: : LG ThinQ
- **Internet Requirements**:
  - Not required to utilize device, but remote control, remote monitoring, software updates, and integration with voice assistants features require internet connectivity through the ThinQ app.[^1]
- **Authentication**
  - User authentication is required to access the ThinQ app. Multi-factor authentication (MFA) is not enforced by default.[^2]
- **Data Transmission Security**
  - The ThinQ app uses encrypted communication protocols HTTPS/TLS for cloud interactions and data transmissions between the device and app.[^2][^8]
- **Physical Security**
  - Standard appliance security applies. Physical access could potentially allow tampering or data extraction.[^2]
- **Storage**
  - The ovens stores essential operational data locally. Usage statistics, preferences, and diagnostics are stored in the cloud via the ThinQ platform.[^3][^8]
- **Data Requirements**
  - No specific bandwidth requirements are disclosed. The oven connects via 2.4GHz Wi-Fi, suitable for standard home broadband connections.[^4][^8]
- **Data Gathering**
  - The ovens collects data such as usage patterns, temperature settings, and diagnostic information to enhance user experience and for maintenance purposes.[^3][^6]
- **Vulnerability Remediation**
  - LG has addressed known vulnerabilities, such as the "HomeHack" issue, by releasing patches and updates to the ThinQ app.[^5][^7]
- **Vulnerability Transparency**
  - LG publishes security bulletins, though disclosures related to ThinQ appliances are less frequent compared to mobile devices. [^5][^7]

[^1]: [LG Range ThinQ Features and Settings](https://www.lg.com/us/support/help-library/lg-range-thinq-features-and-settings--20152599676255)
[^2]: [LG ThinQ - Apps on Google Play](https://play.google.com/store/apps/details?hl=en_US&id=com.lgeha.nuts)
[^3]: [LG ThinQ Smart Home Platform](https://www.lg.com/us/lg-thinq)
[^4]: [Connecting Your Device to the LG ThinQ App via Wi-Fi](https://www.lg.com/us/support/help-library/lg-thinq-connecting-your-device-to-the-lg-thinq-app-via-wi-fi--20153147863991)
[^5]: [Check Point + LG ThinQ Security Partnership](https://www.checkpoint.com/press-releases/check-point-joins-forces-lg-secure-smart-home-devices/)
[^6]: [Smart Appliances Promise Convenience and Innovation.](https://www.consumerreports.org/electronics/privacy/smart-appliances-and-privacy-a1186358482/)
[^7]: [Press Release](https://www.lg.com/us/press-release)
[^8]: [OWNER'S MANUAL - ELECTRIC RANGE](https://images.thdstatic.com/catalog/pdfImages/3a/3a30b356-0070-467b-8632-16136d513971.pdf)
