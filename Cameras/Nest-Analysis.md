# Google Nest Cameras

## Scoring rubric
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | Yes | While there is local storage in cameras it cannot be accessed.  All video must be stored and accessed from the internet. |
| Requires Constant Connection to Company Cloud Infrastructure | Yes | The only location that you can access the videos is from the Google Nest/Home apps, and all video is constantly uploaded there for analysis for events. |
| Data Storage Requirements | Cloud | Local storage is minimal, is used for when there is network or power loss, and cannot be accessed.  All video must be stored in the cloud to be usuable |
| Data Gathering Risk Score | 2 | Google's data gathering is primarily internal, and they do not sell their data to 3rd party entities, although they are one of the largest targets advertising providers.  The more applications that you use in their ecosystem the more data they do gather on you, and the more you are tracked.  There are extensive opt out options that they provide though. |
| Company Vulnerability Remediation Score | 1 | Google purchased Nest back in 2014, and suffered a major breach of all customers 5 years later.  They appear to be on top of their security since then, but you cannot check their updates prior to 2022.  They don't provide any patch notes for their cameras which is interesting. |
| Company Vulnerability Transparency Score | 1 | Their bug bounty program is great and is quite active both from the user and company point of view.  They are lacking in notifications prior to 2022 which is concerning that these started 3 years after their major breach.  They do post all of their updates with the CVE number that can be checked and verified.  They do not have ANY patch notes for their cameras which is a major issue that should be resolved | 

### Total Score: 4

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
  - Google collects data based on the device that you are using, and the more google services that you utilize the more data they will collect[^5].
  - They utilize facial recognition within their camera system, and have location data if you are signed into their services[^5].
  - Utilize Voice and Audio information as well as purchase information to serve targeted ads[^5].
  - This is all tied to the google account you create, and based on device identifiers[^5].
  - Data is not shared without your consent or unless their are legal reasons.  Data can also be shared for external processing but it is not sold off
    - Google does provide some of the largest advertising services on the internet.
  - They do provide options to opt out of the data gathering, but they are straight forward to configure.
    - https://myaccount.google.com/intro/privacycheckup?hl=en_US
[^5]: [Privacy Policy](https://policies.google.com/privacy?hl=en0)
- **Vulnerability Remediation**
  - There does not appear to be any publically available patch notes for their Nest cameras, although other Nest products do have publically available notes.
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

