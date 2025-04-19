# U-tec/UHome/ULTRALOQ Locks
## Analysis
- **Name**: U-tec/UHome/ULTRALOQ
- **Manufacturer**: Utec
- **Country of Origin**: US
- **Platform**: U-Tec
- **Internet Requirements**:
    - Locks can operate in standalone mode, however the application requires Internet to set it up the first time.  [^1]
- **Authentication**
   - Plain username and password.
   - 4 digit PINs are used within the application for certain functions, however they are optional.  
- **Data Transmission Security**
    - Bluetooth only can be used in a failsafe mode and for initial configuration, but is always enabled as well.
    - All devices either have built-in WiFi, or use a Bluetooth to WiFi gateway and HTTPs to cloud services.
    - HTTPs.  
- **Physical Security**
    - Most devices have the option for a backup physical key, local PIN Pad, or local biomtric.
- **Storage**
    - Configuration data is stored in the cloud, such as lock users and password, as well as ACL's for those users.
    - Biometrics are stored locally
    - PINs are stored locally and in the cloud.
- **Data Requirements**
    - Low, but sensitive data; (PINs), ACLs, access logs.
- **Data Gathering**
  - A log is kept of all lock activity in the cloud.
  - Biometrics are stored in the device vs. cloud.
  - Location is required for optional proximity.
- **Vulnerability Remediation**
  - U-Tec has addressed some, but not all common Bluetooth vulnerabilities via firmware updates.
- **Vulnerability Transparency**
  - Previous, but addressed CVEs in Bluetooth personal area network (out of scope) [^2]
  - Additional information on CVE's since the CVE are now gone. [^3]

## Scoring rubric
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | Yes | The lock can operate with limited functionality in Bluetooth only mode after intial setup.   |
| Requires Constant Connection to Company Cloud Infrastructure | No | For full functionality, the device requires Internet connectivity but can operate with limited functionality with Bluetooth only, or with no connectivity via other methods.  Or with PIN or biometric, and as a last resort physical key. |
| Data Storage Requirements | Cloud | Critical data is stored in the cloud and on the device. |
| Data Gathering Risk Score | 3 | Proximity data is optional.  Biometrics stored in the device vs. the Cloud was a wise choice. |
| Company Vulnerability Remediation Score | 3 | U-Tec has released fixes, but continues to ignore general inquiries. |
| Company Vulnerability Transparency Score | 3 | All disclosed vulnerabilities have been common to Bluetooth vs. specific vulnerabilities in the device of their systems. | 

### Total Score: 9

[^1]: [Local Storage of PINs and biomerics](https://ieeexplore.ieee.org/abstract/document/9537052)
[^2]: [Common Bluetooth CVEs](https://app.opencve.io/cve/?vendor=u-tec&product=ultraloq_ul3_bt)
[^3]: [Additional CVE references](https://threatpost.com/smart-lock-turns-out-to-be-not-so-smart-or-secure/146091/)


