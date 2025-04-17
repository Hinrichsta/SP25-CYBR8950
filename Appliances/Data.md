# Appliances


## [ThinQ]([https://store.google.com/category/nest_cams?hl=en-US](https://thinq.developer.lge.com/en/cloud/docs/thinq-connect/overview/))
- 
- ### Concerns
  - 
### Documentation
- Manufacturer Information
  - https://thinq.developer.lge.com/en/cloud/docs/thinq-connect/overview/
  - Security issues Summary
    - https://lgsecurity.lge.com/bulletins/mobile#updateDetails
- Case Studies
  - In 2017, the "HomeHack" vulnerability allowed attackers to remotely control LG smart appliances by exploiting the SmartThinQ app's authentication process. This vulnerability was patched in version 1.9.23 of the app.

### Security 
#### Disclosures
  - 
#### Breaches
  - The vulnerability is an intent redirection in LG ThinQ Service ("com.lge.lms2") in the "com/lge/lms/things/ui/notification/NotificationManager.java" file. This vulnerability could be exploited by a third-party app installed on an LG device by sending a broadcast with the action "com.lge.lms.things.notification.ACTION". Additionally, this vulnerability is very dangerous because LG ThinQ Service is a system app (having android:sharedUserId="android.uid.system" setting). Intent redirection in this app leads to accessing arbitrary not exported activities of absolutely all apps.
    - https://www.nbcnews.com/tech/security/hacked-home-devices-can-spy-you-n814671
  -
    - https://www.cvedetails.com/cve/CVE-2023-44121/
### Notes
  - 
