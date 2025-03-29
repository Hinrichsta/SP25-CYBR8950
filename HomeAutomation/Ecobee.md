# Ecobee Thermostats
## Analysis
- **Name**: Ecobee
- **Manufacturer**: Generac
- **Country of Origin**: US/China
- **Platform**: Ecobee
- **Internet Requirements**:
    - Intial setup via bluetooth, then requires a WiFi connection to Internet for all functions.
    - Can operate with limited functionality via control screen.
- **Authentication**
    - Plain username and password.
    - Family accounts available.  
    - Contractor, and group mode available.
    - Amazon Alexa account (optional)
- **Data Transmission Security**
    - HTTPs
- **Physical Security**
    - There is no physical port.
    - Thermostat can be geofenced to a small range (purpose unknown)
- **Storage**
    - Ecobee stores detailed logs of all device activity and corresponding settings, which are used for [flexible load management data](https://www.ecobee.com/en-us/utilities/).  
- **Data Requirements**
    - Varies based on use.  When Alexa is enabled, the device can function as an Alexa speaker.
- **Data Gathering**
  - Devices can be Amazon Alexa enabled, which is covered in another category.
  - Proximity or pressence information is collected.
  - See Flexible load management under Storage. This data is stored regardless, and shared unless opted out. 
- **Vulnerability Remediation**
  - They appear to have some issues prior to 2022 with a major breach in 2019 that affected every Nest user
    - They had purchased Nest origianlly in early 2014
  - Since 2022 they have been patching vulnerabilities effectively and publically disclosing them
  - There hasn't been a major breach since, but there have been isolated incidents where users report hearing voices coming from their cameras they don't recognize
    - This could be attributed to misconfigured family sharing, or compromised accounts.
- **Vulnerability Transparency**
  - EcoBee has [closed their public api](https://www.ecobee.com/en-us/developers/) to future development and it was not disclosed as to why.

## Scoring rubric
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | No | Can function as a stand alone device |
| Requires Constant Connection to Company Cloud Infrastructure | No | Can still function as a stand alone thermostat. |
| Data Storage Requirements | Cloud | All data is stored in the Cloud. |
| Data Gathering Risk Score | 1 | A lot of data is collected on useage and proximity/pressence.  It knows when you are home and active. |
| Company Vulnerability Remediation Score | 2 | Google purchased Nest back in 2014, and suffered a major breach of all customers 5 years later.  They appear to be on top of their security since then, but you cannot check their updates prior to 2022 |
| Company Vulnerability Transparency Score | 1 | Govee closed their API rather than addressing issues with it. | 

### Total Score: 4
