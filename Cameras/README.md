## [Google Nest](./Nest-Analysis.md)
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | Yes | While there is local storage in cameras it cannot be accessed.  All video must be stored and accessed from the internet. |
| Requires Constant Connection to Company Cloud Infrastructure | Yes | The only location that you can access the videos is from the Google Nest/Home apps, and all video is constantly uploaded there for analysis for events. |
| Data Storage Requirements | Cloud | Local storage is minimal, is used for when there is network or power loss, and cannot be accessed.  All video must be stored in the cloud to be usuable |
| Data Gathering Risk Score | 2 | Google's data gathering is primarily internal, and they do not sell their data to 3rd party entities, although they are one of the largest targets advertising providers.  The more applications that you use in their ecosystem the more data they do gather on you, and the more you are tracked.  There are extensive opt out options that they provide though. |
| Company Vulnerability Remediation Score | 1 | Google purchased Nest back in 2014, and suffered a major breach of all customers 5 years later.  They appear to be on top of their security since then, but you cannot check their updates prior to 2022.  They don't provide any patch notes for their cameras which is interesting. |
| Company Vulnerability Transparency Score | 1 | Their bug bounty program is great and is quite active both from the user and company point of view.  They are lacking in notifications prior to 2022 which is concerning that these started 3 years after their major breach.  They do post all of their updates with the CVE number that can be checked and verified.  They do not have ANY patch notes for their cameras which is a major issue that should be resolved |

### Total Score: 4

<sub>[Privacy Policy](https://policies.google.com/privacy?hl=en0)</sub>  
<sub>[Security Bulletins](https://support.google.com/product-documentation/topic/12823571?hl=en&ref_topic=12974021&sjid=4997332173582231755-NC)</sub>  
<sub>[Nest Camera Video Storage](https://support.google.com/googlenest/answer/9242083)</sub>  
<sub>[Nest Subscription Storage](https://support.google.com/googlenest/answer/9681538/#3-hour-ebr)</sub>  

## [Wyze Cameras](./Wyze-Analysis.md)
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | Yes | There is local storage but it cannot be viewed without using the Wyze app |
| Requires Constant Connection to Company Cloud Infrastructure | Yes | The only location that video can be viewed from is the Wyze app, or the browser web view if you have a subscription |
| Data Storage Requirements | Hybrid | Data can be stored locally, and required if you do not have a subscription.  With a subscription both can be achieved |
| Data Gathering Risk Score | 3 | Overall they only gather data from their products, and through their connections to third party.  They do not sell data in anyway and it is primarily used for internal information.  The Facial recognition data does NOT require consent from those being recorded, but all data is deleted after 30 days.  They do allow for the opting out of their data collection, but it requires sending an email to their support |
| Company Vulnerability Remediation Score | 4 | They did not start disclosing vulnerabilities until about 2022 when they had their first major breach.  Since then they have done better with disclosures and making sure that the information is shared.  Their bug bounty program while existent is lacking. |
| Company Vulnerability Transparency Score | 2 | They do not make any effort to put their vulnerability patches into their patch notes.  Instead they are put into a seperate location in their forums that is difficult to find.  It does appear that it is getting updated, but you wouldn't know it without regularly checking.  They also do not appear to have been disclosing anything before 2022 which is an issue to start. | 

### Total Score: 9

<sub>[Privacy Policy](https://blinkforhome.com/privacy-policy)</sub>  
<sub>[Patch Notes](https://support.blinkforhome.com/en_GB/security-and-app-updates/2016136)</sub>  
<sub>[Storage Options](https://support.blinkforhome.com/en_US/using-your-camera/blink-storage-options)</sub>  

## [Blink Cameras](./Blink-Analysis.md)
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | Yes | Internet is required when viewing videos as a Blink account is required to view all videos. |
| Requires Constant Connection to Company Cloud Infrastructure | Yes | An account is required even when viewing videos in local storage |
| Data Storage Requirements | Cloud | Local storage is an option, but only if specifically configured and video is only backed up to local storage rather than being stored while being recorded.  Otherwise all storage is cloud based |
| Data Gathering Risk Score | 2 | Does not sell data to 3rd party companies, but all data is shared with partner companies.  They are a subsidiary of Amazon as such Amazon has access to all data. |
| Company Vulnerability Remediation Score | 3 | Patches are applied regularly, and of the vulnerabilites that were discovered they were patched promptly.  The same can be said about the breach that they experienced. |
| Company Vulnerability Transparency Score | 2 | THey do not state exactly what was patched in their patch notes, nor are vulnerabilities publically disclosed.  As such there is no transparency to their patching process | 

### Total Score: 7

<sub>[Privacy Policy](https://www.wyze.com/policies/privacy-policy)</sub>  
<sub>[Release Notes](https://support.wyze.com/hc/en-us/articles/360024852172-Release-Notes-Firmware)</sub>  
<sub>[Subscription Plans](https://www.wyze.com/pages/compare)</sub>  
<sub>[Disclosures Listings](/Data.md#disclosures-1)</sub>  

## [Tapo Cameras](./TP-Link-Analysis.md)
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | Hybrid  | Internet connection is required for initial setup, but beyond that the connection is not required beyond that. |
| Requires Constant Connection to Company Cloud Infrastructure | Hybrid | You need to connect for initials setup, and to access and download videos through the app. |
| Data Storage Requirements | Hybrid | Both local and CLoud storage are available, and able to be easily used.  Cloud storage does require a subscription, but you only get a few advantages over local storage |
| Data Gathering Risk Score | 1 | TP-Link actively gathers and sells the data of their users.  They will use their data for targets advertising.  They are also a company based in China, and subject to the Chinese Government |
| Company Vulnerability Remediation Score | 2 | They do regularly patch their products, and make sure to cover disclosed vulnerabilities before the actual disclosure |
| Company Vulnerability Transparency Score | 2 | Their patch notes do not actively share the patches of bugs and vulnerabilities, it is also quite difficult to access the patch notes.  They do share disclosures in CVEs, and periodically share security advisories, but do not actively share things | 

### Total Score: 5

<sub>[TP-Link Privacy Policy](https://privacy.tp-link.com/web/official/privacy-policy?region=US)</sub>  
<sub>[Tapo Care](https://www.tapo.com/us//tapocare/)</sub>  
<sub>[Vulnerabilites List](/Data.md#disclosures-4)</sub>  