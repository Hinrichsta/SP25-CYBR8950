# Kidde Alarms
## Analysis
- **Name**: Kidde
- **Manufacturer**: Carrier Global Corporation
- **Country of Origin**: US/China (unclear)
- **Platform**: Kidde
- **Internet Requirements**:
    - Required Internet connection for remote notifications
- **Authentication**
    - Username and non-case sensitive password
- **Data Transmission Security**
    - HTTPs WiFi (after initial Bluetooth setup)
- **Physical Security**
    - There is no physical port.  
- **Storage**
    - Historical events are stored within the Cloud.
    - For advanced air quality sensors, it is not clear what data is stored since Kidde uses their own proprietary air quality metric.
- **Data Requirements**
    - Minimal
- **Data Gathering**
  - Only the expected data appears to be gathered.
  - Unclear which company or parent company privacy policy applies [^1][^2]
- **Vulnerability Remediation**
  - All reported vulnerabilities were related to the device itself and its core functionality vs. it IoT services.
- **Vulnerability Transparency**
  - The initial products were subject to false alarms and recalled, not because of their IoT alarms but basic traditional alarm functionality. [^3]
  - Kidde alarms have been the subject of my personal research (Josh) because if the lack of public information I can find on them, and the issues I have had with them.

## Scoring rubric
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | No | Can be setup with no connection at all, with limited functionality. |
| Requires Constant Connection to Company Cloud Infrastructure | No | The device can function as a traditional and inter-connected alarm via standard 3 wire systems (interconnect).
| Data Storage Requirements | Cloud | Event data is stored in the Cloud, as well as air quality monitoring data. |
| Data Gathering Risk Score | 4 | Only the required data is collected. |
| Company Vulnerability Remediation Score | 4 | Kidde has addressed product issues, but not faced IoT issues yet. |
| Company Vulnerability Transparency Score | 3 | Given they have addressed product safety issues they score well.  But this product has not been on the market long enough for full IoT analysis.  It is not likely to score well at a later time as Kidde did their own IoT backend rather than use a common platform. | 

### Total Score: 11

[^1]: [Carrier Privacy Policy](https://www.kidde.com/home-safety/en/us/legal/privacy-notice/)  
[^2]: [KGB Privacy](https://www.kidde.com/home-safety/en/us/legal/privacy-notice/)    
[^3]: [Product Recalls](https://www.kidde.com/home-safety/en/us/support/product-alerts/recall-kidde-trusense/)    
