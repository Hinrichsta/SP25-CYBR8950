# Tapo Cameras

## Scoring rubric
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | Hybrid  | Internet connection is required for initial setup, but beyond that the connection is not required beyond that. |
| Requires Constant Connection to Company Cloud Infrastructure | Hybrid | You need to connect for initials setup, and to access and download videos through the app. |
| Data Storage Requirements | Hybrid | Both local and CLoud storage are available, and able to be easily used.  Cloud storage does require a subscription, but you only get a few advantages over local storage |
| Data Gathering Risk Score | 1 | TP-Link actively gathers and sells the data of their users.  They will use their data for targets advertising.  They are also a company based in China, and subject to the Chinese Government |
| Company Vulnerability Remediation Score | 2 | They do regularly patch their products, and make sure to cover disclosed vulnerabilities before the actual disclosure |
| Company Vulnerability Transparency Score | 2 | Their patch notes do not actively share the patches of bugs and vulnerabilities, it is also quite difficult to access the patch notes.  They do share disclosures in CVEs, and periodically share security advisories, but do not actively share things | 

### Total Score: 5

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
  - Some Cameras do use a USB Type C charging cable
    - It is only covered.[^8]
[^4]: [Camera Specifications](https://www.tp-link.com/us/support/faq/3395/)
[^8]: [Camera Quick Start Guide](https://static.tp-link.com/upload/manual/2024/202404/20240403/7106511087_Tapo%20C410(US)1.0_QIG.pdf)
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
  - Tapo is a company under TP-Link and uses their Privacy Policy
  - Gathers Data relating to location, how you got to their website, and what you access on their site[^6].
  - They also gather data related to your account, and will get data from partners[^6].
  - They utilize your information for targeted advertising and sell/share your data with their partnerts[^6].
    - Targeted advertising includes their own and 3rd party.  
      - This includes Google, Amazon, and Meta [^11].  
  - To opt out of their data collection you must contact their support to remove data they have[^6].
    - email privacy.us@tp-link.com 
[^6]: [TP-Link Privacy Policy](https://privacy.tp-link.com/web/official/privacy-policy?region=US)
[^11]: [Do Not Sell My Info](https://www.tp-link.com/us/about-us/privacy/do-not-sell-my-info/)
- **Vulnerability Remediation**
  - Firmware Releases appear to happen every 1-4 months, and isn't on a consistent Schedule[^7]
  - Their Patch notes are mostly related to improvements and not patches and big fixes
  - They do appear to post security advisories when patching large vulnerabilities, and recommend upgradings[^9].  
[^7]: [Firmware Release notes for C402](https://www.tp-link.com/us/support/download/tapo-c402/#Firmware-Release-Notes)
[^9]: [Security Advisory](https://www.tp-link.com/us/support/faq/3722/)
- **Vulnerability Transparency**
  - Able to find 1 Security Advisory relating to cameras on their Website[^9]
  - CVEs for cameras are shared and patches for them are shown[^10]
    - This does not appear to be shared directly in their patch notes
  - No major breaches have been seen relating to Tapo, but TP-Link itself has had breaches in the past.
[^10]: [Vulnerabilites List](/Data.md#disclosures-4)