# Govee Temperature and Other sensors (water, weather, etc.)
## Analysis
- **Name**: Govee, Govee Life
- **Manufacturer**: Govee
- **Country of Origin**: China
- **Platform**: Govee, Govee Life
- **Internet Requirements**:
    - Some devices can operate with more limited functionality in Bluetooth only mode.  
    - Requires an Internet connection to Govee Life to use full functionality via a Bluetooth to WiFi gateway (for power reasons).
- **Authentication**
    - Plain username and password.  
- **Data Transmission Security**
    - For Internet, all communication is HTTPs via an open API (with limited documentation) for most new devices
    - But older Govee devices [do not use encryption](https://community.home-assistant.io/t/security-concerns-with-govee-devices-seeking-solutions-and-alternatives-h5072-h5075/683314/2), and instead Govee has implemented a device safety feature.  This features, which is not enabled by default means that once a Govee device has connected to one installation of the app, it can only connect to that copy of the running app.  This prevents other control devices on your network from connecting to it, but does not prevent network sniffing of the plain text data.  This is a strange work-around for not using encryption - likely related to the low compute power of the sensors and gateway.  The Govee API gateway however does require SSL.
- **Physical Security**
    - There is no physical port.  
- **Storage**
  - Govee stores some data locally, and all data in the cloud, which is not disclosed clearly and was discovered via testings (delete the app and some data comes back).
- **Data Requirements**
    - Low, generally non sensitive data.
    - But, Govee devices are [considered to be rather chatty](https://hal.science/hal-04936304/), despite not being ask to do anything which is concerning with HTTPs devices as it is not known what they are doing.  
- **Data Gathering**
  - All possible permissions are requested by the application regardless of need as the app can control many different devices.  
- **Vulnerability Remediation**
    - [Govee CVE - CVE-2023-3612](https://nvd.nist.gov/vuln/detail/CVE-2023-3612)  
- **Vulnerability Transparency**
  - Very basic [Privacy Policy](https://us.govee.com/pages/privacy-policy?srsltid=AfmBOoos77IPMaQoDdTlP_Xt3Wt2d-gZVVijfFM5jtmRVmissv2iA5hi) which is very minimal compared to Tuya.

## Scoring rubric
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | No | While local connectivity is an option after intial setup, most users would not chose this option as it is not the default. |
| Requires Constant Connection to Company Cloud Infrastructure | No | As noted above, for most users this would be a yes.  While the device can be used with just Bluetooth, strange app behavior can occur as this is not the expected configuration. |
| Data Storage Requirements | Cloud | It is not entirely clear how much data is stored locally vs. cloud, and how it is synched.  This is likely do to the Bluetooth connection alternative.  They claim to only store 12 months of data, but it has been reported that it is stored longer.  Testing of this statement will be complete May 1st. |
| Data Gathering Risk Score | 4 | The device's purpose is to collect data, and because of the hardware, it only collects the data it has disclosed. |
| Company Vulnerability Remediation Score | 1 | Like Tuya, Govee has not disclosed vulnerabilities of addressed them and instead focused on new products. |
| Company Vulnerability Transparency Score | 1 | Govee has never disclosed vulnerabilities in products. | 

### Total Score: 6
