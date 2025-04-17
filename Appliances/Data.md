# Appliances


## [ThinQ]((https://thinq.developer.lge.com/en/cloud/docs/thinq-connect/overview/)
- Smart appliances like refridgerators use LG’s ThinQ platform and it is known as one of the leading ecosystems for connected appliances. It allows users to control and monitor them remotely via the ThinQ mobile app. Integrating features like voice assistants is also supported.
- Since these appliances require a connection to the internet, most of the data and functionality is cloud-based. The features are also only managed by the Mobile App and this inherits various concerns about privacy, data security, and long-term support.
  
- ### Concerns
  - There is limited publicly available documentation of widespread breaches, though LG devices are sometimes included in broader IoT botnet scans or theoretical attack studies.
  - LG ThinQ devices require connection to the LG ThinQ app for full functionality.
  - The ecosystem collects operational data from the appliances and sends it to the cloud.
  - Most ThinQ appliances are not accessible without an LG account and an internet connection.
  - Integration with smart assistants like Google and Alexa expands usability but increases the surface area for potential breaches.

Long-term software update support and patching cadence for older appliances is unclear.
### Documentation
- Manufacturer Information
  - ThinQ Developer Docs
    - https://thinq.developer.lge.com/en/cloud/docs/thinq-connect/overview/
  - Security issues Summary
    - https://lgsecurity.lge.com/bulletins/mobile#updateDetails
  - Privacy Policy
    - https://privacy.us.lg.com/policies
- Case Studies
  - In 2017, the "HomeHack" vulnerability allowed attackers to remotely control LG smart appliances by exploiting the SmartThinQ app's authentication process. This vulnerability was patched in version 1.9.23 of the app.

### Security 
#### Disclosures
  - LG does publish security bulletins but typically only for mobile devices. Disclosures related to ThinQ appliances are rare and often buried in broader vulnerability summaries. They seem to hide or obfuscate the vulnerabilities in Appliances, but do have reguarly schedule updates and suggest you stay within 90 days of all new patches.
    - https://lgsecurity.lge.com/bulletins/homeappliance
  - Check Point Press Releases an article highlighting a collaboration to help secure the ThinQ Mobile App. This helps to show that LG is striving to secure the access to IoT appliances.
    - https://www.checkpoint.com/press-releases/check-point-joins-forces-lg-secure-smart-home-devices/
  - Recent Relevant Disclosure:
    - CVE-2023-44121: Intent redirection vulnerability in LG ThinQ Service. This system-level vulnerability allows a malicious third-party app to access arbitrary, non-exported activities from all installed apps, posing a serious threat.
#### Breaches
  - The vulnerability is an intent redirection in LG ThinQ Service ("com.lge.lms2") in the "com/lge/lms/things/ui/notification/NotificationManager.java" file. This vulnerability could be exploited by a third-party app installed on an LG device by sending a broadcast with the action "com.lge.lms.things.notification.ACTION". Additionally, this vulnerability is very dangerous because LG ThinQ Service is a system app (having android:sharedUserId="android.uid.system" setting). Intent redirection in this app leads to accessing arbitrary not exported activities of absolutely all apps.
    - https://www.nbcnews.com/tech/security/hacked-home-devices-can-spy-you-n814671
      
### Notes
  - [Bug Bountry program](https://lgsecurity.lge.com/rewards)


## []()
- 
  
- ### Concerns
  - 
### Documentation
- 

### Security 
#### Disclosures
  - 
#### Breaches
  - 
      
### Notes
  - [Bug Bountry program]()


## []()
- 
  
- ### Concerns
  - 
### Documentation
- 

### Security 
#### Disclosures
  - 
#### Breaches
  - 
      
### Notes
  - [Bug Bountry program]()


## []()
- 
  
- ### Concerns
  - 
### Documentation
- 

### Security 
#### Disclosures
  - 
#### Breaches
  - 
      
### Notes
  - [Bug Bountry program]()
