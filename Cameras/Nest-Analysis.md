# Google Nest Cameras
## Analysis
- **Name**: Google Nest Cameras
- **Manufacturer**: Google
- **Country of Origin**: US Owned Company | Manufactured in Taiwan and Malaysia
- **Platform**: Google Home
- **Internet Requirements**:
    - Requires internet connection to access all video[^1].
    - Requires connection to Google Cloud Services to access all videos[^1].  
[^1]: [Nest Camera Video Storage](https://support.google.com/googlenest/answer/9242083)
- **Authentication**
    - Nest account can require MFA, but doesn't by default.
    - There is family sharing, which anybody can be invited to view cameras.
- **Data Transmission Security**
    - Cameras can use WEP, WPA, WPA2, WPA3 encryption for Wireless[^2].
    - Only communicates over Wireless[^2].
- **Physical Security**
    - There is no physical port on the Main Outdoor/Indoor Camera Line.
      - Cameras use a magnetic connector to power the camera[^2].  
[^2]: [Camera Technical Specifications](https://support.google.com/googlenest/answer/9259110?hl=en#zippy=%2Cnest-cam-outdoor-or-indoor-battery)
- **Storage**
    - Data is stored in the cloud[^1].
    - 3 tiers of data storage at a subscription price[^3].
        - Free - 3 hours of video event storage.
        - Nest Aware - 30 days of video event storage.
        - Nest Aware + - 60 days of video event storage and 10 days of 24/7 video storage.
    - Most cameras have local storage[^1].
        - Used for when network is lost.
        - Cannot be accessed.
[^3]: [Nest Subscription Storage](https://support.google.com/googlenest/answer/9681538/#3-hour-ebr)
- **Data Requirements**
    - 1-4 Mbps/camera[^4]  
[^4]: [Camera Bandwidth](https://support.google.com/googlenest/answer/9245832#zippy=%2Cupload-bandwidth-used-by-cameras-and-doorbells%2Cnest-cam-battery-and-nest-cam-wired)
- **Data Gathering**
  - Google is one of the largest internet companies out there and is notorious for gathering as much data on you as possible.
  - They utilize facial recognition within their camera system, and have location data if you are signed into their services[^5].
  - Utilize Voice and Audio information as well as purchase information to serve targeted ads.
  - Expect everything that you do within this ecosystem to be monitored, analyzed and stored.  
[^5]: [Privacy Policy](https://policies.google.com/privacy?hl=en0)
- **Vulnerability Remediation**
  - They appear to have some issues prior to 2022 with a major breach in 2019 that affected every Nest user[^6].
    - They had purchased Nest origianlly in early 2014.
  - Since 2022 they have been patching vulnerabilities effectively and publically disclosing them[^7].
  - There hasn't been a major breach since, but there have been isolated incidents where users report hearing voices coming from their cameras they don't recognize.
    - This could be attributed to misconfigured family sharing, or compromised accounts.  
[^6]: [Nest 19 Security Breach](https://www.popularmechanics.com/technology/security/a26214078/google-nest-hack-warning/)
[^7]: [Security Bulletins](https://support.google.com/product-documentation/topic/12823571?hl=en&ref_topic=12974021&sjid=4997332173582231755-NC)
- **Vulnerability Transparency**
  - Has a bug bounty program put out by the company where they regularly payout reports and and very transparent with the program.[^8]
  - Each major security vulnerability patch is clearly posted and documented for users to find.[^7]
    - CVE reports are posted and addressed with clarity.
[^8]: [Bug Bounty Program](https://bughunters.google.com/about/rules/android-friends/6171833274204160/android-and-google-devices-security-reward-program-rules)

## Scoring rubric
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | Yes | While there is local storage in cameras it cannot be accessed.  All video must be stored and accessed from the internet. |
| Requires Constant Connection to Company Cloud Infrastructure | Yes | The only location that you can access the videos is from the Google Nest/Home apps, and all video is constantly uploaded there for analysis for events. |
| Data Storage Requirements | Cloud | Local storage is minimal, is used for when there is network or power loss, and cannot be accessed.  All video must be stored in the cloud to be usuable |
| Data Gathering Risk Score | 1 | Google is always gathering data, and notoriously gathers as much as possible.  They utilize video sent to their cloud to grow their services and to gather data on their users.  Once you are a part of the ecosystem everything you do with that account is tracked even beyond just the cameras |
| Company Vulnerability Remediation Score | 3 | Google purchased Nest back in 2014, and suffered a major breach of all customers 5 years later.  They appear to be on top of their security since then, but you cannot check their updates prior to 2022 |
| Company Vulnerability Transparency Score | 3 | Their bug bounty program is great and is quite active both from the user and company point of view.  They are lacking in notifications prior to 2022 which is concerning that these started 3 years after their major breach.  They do post all of their updates with the CVE number that can be checked and verified. | 

### Total Score: 7