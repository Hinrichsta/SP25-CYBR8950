# Smart Fridge
## Analysis
- **Name**: Samsung Family Hub Refrigerator​
- **Manufacturer**: Samsung Electronics​
- **Country of Origin**: South Korea​
- **Platform**: Tizen OS​
- **Internet Requirements**:
    - Active Internet Required: Calendar, Monitoring, Media Streaming, and Notifications
- **Authentication**
    - Samsung App Authentication (Samsung Account Credentials)
- **Data Transmission Security**
    - HTTPS - SSL/TLS X.509 certificates
- **Physical Security**
    - Standard appliance security with screws and accessible parts. Could lead to tampering or data theft with physical access. 
- **Storage**
    - Stores locally on internal disk and in cloud. Stores Calendar info and shopping lists.. 
- **Data Requirements**
    - Samsung does not specify exact bandwidth requirement, but they do suggest a stable broadband connection is recommended to support media streaming, updates, and other connected features.
    - Connects only to 2.4 GHz Wi-Fi networks, and does not support 5 GHz bands.
- **Data Gathering**
    - Collecting and storing food habits, shopping information, and other personal data that raises concerns.  
- **Vulnerability Remediation**
    - Samsung now uses a security measure called Samsung Knox. This has allowed them to achieve Diamond-level security verification from UL Solutions for its appliances.​
- **Vulnerability Transparency**
    - Samsung has addressed reported vulnerabilities within a reasonably expected timeframe. They also recommend users keep their devices updated to the latest firmware.​
- **Sources**
    - https://blog.digital-forensics.it/2020/12/a-journey-into-iot-forensics-episode-1.html
    - Ethical Hacking of a Smart: Fridgehttps://www.diva-portal.org/smash/get/diva2:1596057/FULLTEXT01.pdf
    - https://www.techradar.com/computing/heres-why-samsung-has-built-the-worlds-most-secure-smart-fridge-and-a-host-of-other-super-secure-appliances
    - https://www.samsung.com/us/support/troubleshooting/TSG01001816/
    - https://www.samsung.com/us/support/troubleshooting/TSG01109770/

| Risk Category                  | Samsung Fridge | Beko Fridge | LG Oven | AEG Oven |
|--------------------------------|----------------|-------------|---------|----------|
| Internet Required              | Yes            | Partial     | Yes     | Partial  |
| Cloud Dependency               | Yes            | Partial     | Yes     | Partial  |
| Data Storage Requirement       | Cloud          | Hybrid      | Cloud   | Hybrid   |
| Data Gathering Risk (1–5)      | 2              | 4           | X       | X        |
| Vulnerability History (1–5)    | 2              | 5           | X       | X        |
| Transparency (1–5)             | 4              | 4           | X       | X        |
| **Total Risk Score**           | **8**          | **13**      | **XX**  | **XX**   |
