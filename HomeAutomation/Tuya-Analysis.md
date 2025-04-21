# Tuya/SmartLife switches and bulbs
## Scoring rubric
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | Yes | There is no local communication option past setup.   |
| Requires Constant Connection to Company Cloud Infrastructure | Yes | All control is via API calls to the cloud service.   |
| Data Storage Requirements | Cloud | You can not opt out of usage collection, even if you are not using it the features that require it.   |
| Data Gathering Risk Score | 4 | The data that is gathered is not sensitive, but this is the nature of the product. |
| Company Vulnerability Remediation Score | 1 | They seem to have remediated issues via new products vs. patching or updating firmware on existing products as evidence by the various backends. |
| Company Vulnerability Transparency Score | 1 | Tuya has never disclosed vulnerabilities in products. | 
### Total Score: 6

## Analysis
- **Name**: Tuya
- **Manufacturer**: Tuya
- **Country of Origin**: China[^1]
- **Platform**: SmartLife (most common) or Tuya (same) [^2]
- **Internet Requirements**:
    - Initial setup via Bluetooth, then requires a WiFi connection to Internet for all functions.  
    - Requires an Internet connection for all useful or expected operations.  
- **Authentication**
    - Username and password.  
- **Data Transmission Security**
    - HTTP or HTTPs, this depends on the model of device you have purchased as older devices are HTTP only and use HTTP only Tuya services.  
- **Physical Security**
    - These devices can usually be flashed with third party firmware which is often down to disable the WiFi feature.
    - No physical connection (port) other than the AC electrical connection.
- **Storage**
    - These devices don't collect data by design, however usage information is collected in the cloud for energy use metrics.  
- **Data Requirements**
    - Low, generally non sensitive data.
- **Data Gathering**
  - All possible permissions are requested by the application regardless of need as the app can control many different devices.  
  - Overall usage information is collected, but only used if the end user wants to do energy consumption metrics.  [^3]
- **Vulnerability Remediation**
  - Firmware is never updated past the initial setup.  
- **Vulnerability Transparency**
  - Numerous CVE's - Example: CVE-2024-3764 Detail] [^4]
  - Researchers have  urged the US government to ban Tuya devices over privacy concerns. [^5]


[^1]: [Tuya SaaS Platform](https://www.atlantis-press.com/proceedings/icssed-22/125973899)  
[^2]: [World's Leading Supplier of smart home devices](https://www.tuya.com/platform/vas/works-with)
[^4]: [CVE-2024-3764](https://nvd.nist.gov/vuln/detail/CVE-2024-3764)
[^5]: [Concerns of Chinese SaaS Cloud Platorms](https://www.voanews.com/a/east-asia-pacific_voa-news-china_cybersecurity-experts-worried-chinese-firms-control-smart-devices/6209815.html)  
[^3]: [Privacy Policy](https://images.tuyacn.com/app/smart/Privacy_Policy_en.html)
