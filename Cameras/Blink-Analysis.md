# Blink Cameras
## Analysis
- **Name**: Blink
- **Manufacturer**: Amazon
- **Country of Origin**: United States
- **Platform**: Blink Home Monitor | Can be connected to Amazon Alexa
- **Internet Requirements**:
  - Requires internet connection[^1].
    - A Sync Module is required for most cameras make the connection, very few products don't need to sync[^2].
  - Requires connection to Blink CLoud to access videos.
    - Clips backed up can be viewed with a computer[^3].  
[^1]: [Blink System Requirements](https://support.blinkforhome.com/en_US/f-a-q/system-requirements)
[^2]: [Sync Module FAQ](https://support.blinkforhome.com/en_GB/f-a-q/sync-module-xr-faq)
[^3]: [Blink Storage Options](https://support.blinkforhome.com/en_US/using-your-camera/blink-storage-options)
- **Authentication**
  - Requires MFA for accounts[^4].
    - Only does Text and Phone Call based authentication.
  - Sharing a system is done by sharing account[^5].  
[^4]: [Account MFA](https://support.blinkforhome.com/en_US/account-and-login/multiple-factor-security)
[^5]: [Sharing accounts](https://support.blinkforhome.com/en_GB/managing-your-blink-account/how-to-manage-devices)
- **Data Transmission Security**
  - Cameras are connected through WiFi[^6].  
    - Utilize SSL[^7] to encrypt data transmission
[^6]: [System Requirements](https://support.blinkforhome.com/en_US/f-a-q/system-requirements)  
[^7]: [Privacy Policy](https://blinkforhome.com/privacy-policy)
- **Physical Security**
  - Outdoor Cameras are battery powered and utilize WiFi for data transfers[^8].
  - Mini Cameras are powered by a USB-C cable and WiFi for data transfers[^9].  
  - Devices do not store any data on them, and is directly transmitted to the sync module and then cloud. 
[^8]: [Outdoor Camera Techical Specifications](https://support.blinkforhome.com/en_GB/tech-specs-outdoor4/outdoor4-camera-tech-specs)
[^9]: [Mini2 Camera Technical Specifications](https://support.blinkforhome.com/en_GB/faq-mini-2/mini-2-faq)
- **Storage**
  - All data is transfered to the cloud, and requires a subscription for the storage[^10].
  - Data can be backed up to a USB device or MicroSD cared (Depending on sync module)[^10].
    - Stored video can be viewed on a computer, but requires an account to view[^10].  
  - Live video can be viewed without a subscription, and Local Storage can be used.
  - Both plan options allow for 60 days of video storage[^11].  
[^10]: [Storage Options](https://support.blinkforhome.com/en_US/using-your-camera/blink-storage-options)
[^11]: [Subscription Options](https://support.blinkforhome.com/en_GB/subscriptions-faq/subscription-faq)
- **Data Requirements**
  - Requires a 2mbps upload speed per blink device[^1]
- **Data Gathering**
  - Gathers basic information regarding their account, where they log in from, and location of devices[^7].
  - Does not explicitly sell personal data, but allows third party access when working with other businesses[^7].
    - Is a subsidiary of Amazon[^12].
  - Does provide opt out options of some of the data gathering, but requires you to contact support to turn it off[^7].
    - Does mention that opting out may reduce features of your account and devices[^7].
[^12]: [Blink About Us](https://blinkforhome.com/about-us)
- **Vulnerability Remediation**
  - Patch notes are minimal, and do not state anything about remediating vulnerabilities[^13]. 
  - They do appear to have a monthly patching cycle with only a few months missed periodically[^13]
  - One Major Breach in 2019 that was discovered[^14].  
[^13]: [Patch Notes](https://support.blinkforhome.com/en_GB/security-and-app-updates/2016136)
[^14]: [Vulnerability Discovery by Tenable](https://investors.tenable.com/news-releases/news-release-details/tenable-research-finds-new-vulnerabilities-popular-blink-smart)
- **Vulnerability Transparency**
  - Only found a single Vulnerability in the CVE database, from 2018[^15].
[^15]: [CVE-2018-20161](https://nvd.nist.gov/vuln/detail/CVE-2018-20161)

## Scoring rubric
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | Yes | Internet is required when viewing videos as a Blink account is required to view all videos. |
| Requires Constant Connection to Company Cloud Infrastructure | Yes | An account is required even when viewing videos in local storage |
| Data Storage Requirements | Cloud | Local storage is an option, but only if specifically configured and video is only backed up to local storage rather than being stored while being recorded.  Otherwise all storage is cloud based |
| Data Gathering Risk Score | 2 | Does not sell data to 3rd party companies, but all data is shared with partner companies.  They are a subsidiary of Amazon as such Amazon has access to all data. |
| Company Vulnerability Remediation Score | 3 | Patches are applied regularly, and of the vulnerabilites that were discovered they were patched promptly.  The same can be said about the breach that they experienced. |
| Company Vulnerability Transparency Score | 2 | THey do not state exactly what was patched in their patch notes, nor are vulnerabilities publically disclosed.  As such there is no transparency to their patching process | 

### Total Score: 7