# Tuya/SmartLife switches and bulbs
## Analysis
- **Name**: Tuya
- **Manufacturer**: Tuya
- **Country of Origin**: China
- **Platform**: SmartLife (most common) or Tuya (same)
- **Internet Requirements**:
    - Intial setup via bluetooth, then requires a WiFi connection to Internet for all functions.  
    - Requires an Internet connection for all operations.  
- **Authentication**
    - Plain username and password.  
- **Data Transmission Security**
    - HTTP or HTTPs, this depends on the model of device you have purchased as older devices are HTTP only and use HTTP only Tuya services.  
- **Physical Security**
    - These devices can usually be flashed with third party firmware.
    - But no physical connection (port) other than the AC electrical connection.
- **Storage**
    - These devices don't collect data per say, however useage information is collected in the cloud for energy use metrics.  
- **Data Requirements**
    - Low, generally non sensitive data.
- **Data Gathering**
  - All possible permissions are requested by the application regardless of need as the app can control many different devices.  
  - Overall usage infomration is collected, but only used if the end user wants to do enegy consumption metrics.  
- **Vulnerability Remediation**
  - Firmware is never updated past the intial setup.  
- **Vulnerability Transparency**
  - Numerous CVE's - [Example: CVE-2024-3764 Detail](https://nvd.nist.gov/vuln/detail/CVE-2024-3764)
  - Researchers have [urged the US government] (https://www.voanews.com/a/east-asia-pacific_voa-news-china_cybersecurity-experts-worried-chinese-firms-control-smart-devices/6209815.html) to ban Tuya devices over privacy concerns.
## Scoring rubric
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | Yes | There is no local commmunication option past setup.   |
| Requires Constant Connection to Company Cloud Infrastructure | Yes | All control is via API calls to the cloud service.   |
| Data Storage Requirements | Cloud | You can not opt out of useage collection, even if you are not using it the features that require it.   |
| Data Gathering Risk Score | 4 | The data that is gathered is not sensitive, but this is the nature of the product. |
| Company Vulnerability Remediation Score | 1 | They seem to have remdiated issues via new products vs. patching or updating firmware on existing products as evidence by the various backends. |
| Company Vulnerability Transparency Score | 1 | Tuya has never disclosed vulnerabilities in products. | 

### Total Score: 6
