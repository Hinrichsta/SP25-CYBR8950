# Ecobee Thermostats
## Scoring rubric
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | Yes | But can still function as a stand alone device as a standard non-smart thermostat.   |
| Requires Constant Connection to Company Cloud Infrastructure | Yes | Can still function as a stand alone thermostat. |
| Data Storage Requirements | Cloud | All data is stored in the Cloud. |
| Data Gathering Risk Score | 1 | A lot of data is collected on usage and proximity/presence.  It knows when you are home and active. |
| Company Vulnerability Remediation Score | 2 | Google purchased Nest back in 2014, and suffered a major breach of all customers 5 years later.  They appear to be on top of their security since then, but you cannot check their updates prior to 2022.   |
| Company Vulnerability Transparency Score | 1 | Govee closed their API rather than addressing issues with it. | 

### Total Score: 4

## Analysis
- **Name**: Ecobee
- **Manufacturer**: Generac
- **Country of Origin**: US/China
- **Platform**: Ecobee
- **Internet Requirements**:
    - Initial setup via Bluetooth, then requires a WiFi connection to Internet for all functions.
    - Can operate with limited (basic)functionality via control screen and no connection (including bluetooth)
- **Authentication**
    - Plain username and password.
    - Family sharing accounts  
    - Contractor, and group mode available.
    - Amazon Alexa account (optional).  
- **Data Transmission Security**
    - HTTPs
- **Physical Security**
    - There is no physical port.
    - Thermostat can be geofenced to a small range (purpose unknown but perhaps physical theft).  
- **Storage**
    - Ecobee stores detailed logs of all device activity and corresponding settings, which are used for flexible load management data.  [^1] [^2]
- **Data Requirements**
    - Varies based on use.  When Alexa is enabled, the device can function as an Alexa speaker/microphone (covered with cameras).
- **Data Gathering**
  - Devices can be Amazon Alexa enabled, which is covered in another category but opens up a whole other realm of data collection.
  - Proximity or presence information is collected. [^3]
  - See Flexible load management under Storage. This data is stored regardless, and shared unless opted out. 
- **Vulnerability Remediation**
  -  To many CVEs to list. [^4]
- **Vulnerability Transparency**
  - EcoBee has closed their public api to future development and it was not disclosed as to why, but there are backdoors which is bothersome. [^5] [^1]

[^1]: [Flexible load management](https://www.ecobee.com/en-us/utilities/)
[^2]: [Beestat example](https://app.beestat.io/)
[^3]: [Proximaty sensing concerns](https://ijitra.com/index.php/ijitra/article/view/48/39)  
[^4]: [CVE list](https://app.opencve.io/cve/?vendor=ecobee)  
[^5]: [Closed API and end of Developer Progran](https://www.ecobee.com/en-us/developers/)  



