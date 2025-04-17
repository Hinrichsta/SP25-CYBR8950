# Tapo Cameras
## Analysis
- **Name**: Tapo
- **Manufacturer**: TP-Link
- **Country of Origin**: China
- **Platform**: TP-Link Tapo
- **Internet Requirements**:
  - Requires internet for initial configuration, but can be viewed locally without the app through the set up of a viewing application[^1].  
[^1]: [Viewing without Internet](https://www.tapo.com/us/faq/34/)
- **Authentication**
  - Tapo account is required to set up cameras
  - MFA is not automatically configured when creating account and must be manually setup[^2]
    - Only utilizes Email MFA, which is considered insecure.
  - Cameras can be shared with out Tapo accounts, and invites are sent through the app only[^6].  
[^2]: [Tapo Account MFA](https://www.tp-link.com/us/support/faq/3395/)
[^6]: [Sharing Tapo Devices](https://www.tapo.com/us/faq/40/)
- **Data Transmission Security**
  - Requires networks with WPA or WPA2 wireless encryption[^3]  
  - Utilize AES 128-bit encryption with SSL to encrypt data during transfer[^3]
  - Some cameras do utilize and ethernet connection.
[^3]: [General Tapo Questions](https://www.tp-link.com/us/support/faq/2742/)
- **Physical Security**
  - Cameras have a MicroSD card Slot that supports up to a 512GB card[^4].
    - SD card slot is easily accessible on most cameras
  - Cameras use a Built in Battery which is rechargable through a Solar Panel, or through a power adapter[^4]  
[^4]: [Camera Specifications](https://www.tp-link.com/us/support/faq/3395/)
- **Storage**
  - Video can be locally stored using a MicroSD card[^4]
    - Locally stored video can be accessed through the app
  - Optional Cloud Storage for up to 30 days of video storage[^5]  
  - All Videos can be downloaded through that Tapo App
[^5]: [Tapo Care](https://www.tapo.com/us//tapocare/)
- **Data Requirements**
  - Bandwidth requirements vary, but requires 5mbps for live streaming video[^3]
    - Can live stream up to 4 cameras from one app.
    - Other users can also stream at the same time.
- **Data Gathering**
  - a
- **Vulnerability Remediation**
  - a
- **Vulnerability Transparency**
  - a

## Scoring rubric
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection |  |  |
| Requires Constant Connection to Company Cloud Infrastructure |  |  |
| Data Storage Requirements |  |  |
| Data Gathering Risk Score |  |  |
| Company Vulnerability Remediation Score |  |  |
| Company Vulnerability Transparency Score |  |  | 

### Total Score: 