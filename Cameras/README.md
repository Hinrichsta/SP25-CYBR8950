# Security Cameras
Security cameras a common commodity now a day and are used just about everywhere.  The most common place is the doorbell, as a doorbell camera is easy to set up and use.  Since the internet is ubiquitious that also means that you don't need to have a device to store all of the recordings, it can all be stored on the cloud.  This bring about a lot of different issues that aren't really looked at.  

All of the security cameras that we look at have their own apps that are required to function.  Most of them do integrate with orther smart home applications, but only for added functionality with home assisstants like Google and Alexa.

## [Google Nest](https://store.google.com/category/nest_cams?hl=en-US)
- Google is one of the largest internet companies out there, and they provide one of the major smarthome apps and integrations on the market.  This also means that they have some of the most data collection and information out there.  
- All of their data is stored on their proprietary cloud platform, and is developed to run as their system.
- They are very efficient at putting out patches for their products and for disclosing vulernabilities.
- ### Concerns
  - They are well known for collecting as much data as possible
  - Their Devices require connection to their Google Home/Nest smart apps.
### Documentation
- Manufacturer Information
  - https://policies.google.com/privacy?hl=en
  - https://support.google.com/googlenest/answer/9681538/#3-hour-ebr
  - https://support.google.com/googlenest/answer/9242083
  - https://safety.google/nest/#cameras
  - [Nest Aware (Subscription for Data Storage)](https://store.google.com/product/nest_aware?hl=en-US)
- Case Studies
  - https://www.diva-portal.org/smash/record.jsf?pid=diva2%3A1464437&dswid=6664
  - https://www.tandfonline.com/doi/abs/10.1080/15295036.2022.2143838

## [Wyze](https://www.wyze.com/)
- They are a newer company to the game, having been founded in 2017 specifically focusing on their cameras.  They have also expanded into further smarthome and lifestyle products to augment their brand.
- They have integrations with Smart Home applications, but it is fairly limited opting to require their app for most functionality
- They appear to have a wide variety of options for the entire home, and focus on providing cheap and effective solutions.  They do require a subscription for all of their cameras to have most useful functionalities
  - ### Concerns
    - The subscription model that they provide is fairly predatory considering if you just buy the camera you get minimal functionality.  The best you can do is stream your camera's local storage and all notifications have a 5 minute delay
    - Their security Advisories, while published, are horribly formatted and don't provide a lot of information beyond simple "Fixed X"
### Documentation
- [Manufacturer Information](https://www.wyze.com/pages/security-trust)
  - [Data Storage](https://www.wyze.com/pages/compare)
  - [Privacy Statement](https://www.wyze.com/policies/privacy-policy)
  - [Security Certificate](https://www.securitymetrics.com/site_certificate?id=1837364&tk=ea58e3f46110f7399e03713cf5b8dc55)
  - [Security Advisorys](https://forums.wyze.com/t/security-advisory/289256)
- Case Studies
  - https://engrxiv.org/preprint/view/3079
  - https://escs.vip.gatech.edu/sites/default/files/2025-01/Wyze_Fall_2024_Final_Paper.pdf

## [Blink](https://blinkforhome.com/)\https://ring.com/collections/home-security-cameras
- Blink security cameras are the newer product of security cameras mostly replacing Amazon's Ring cameras.  While Ring cameras still exist this is what they are focusing on going forward and do not appear to be making the branding of this as obviously connected to Amazon.
- They do appear to be open source and utilize the GPL2 license
- The overall data collection as laid out by their privacy policy appears to be fairly minimal and is one of the least invasive ones of those looked at
- ### Concerns
  - These are from Amazon another large company that is known for its data collection.  While the cameras and app themselves do not appear to collect as much data, they do state that they get data and share data with their partners.
  - They do not lay out any security advisories or past vulnerabilities on their website nor do their release notes provide much in the way of useful information other than "Bug Fixes"
### Documentation
- Manufacturer Information
  - https://support.blinkforhome.com/
    - https://blinkforhome.com/safety-and-compliance
    - https://support.blinkforhome.com/en_US/security-and-app-updates/2016136
  - https://blinkforhome.com/privacy-policy
  - https://blinkforhome.com/video-storage
- Case Studies
  - https://dl.acm.org/doi/abs/10.1145/3555125
  - https://www.tandfonline.com/doi/full/10.1080/09505431.2021.1983797

## [TP-Link](https://www.tp-link.com/us/home-networking/cloud-camera/)
- TP-Link is a company well known for their networking systems, being one of the cheaper providers of routers and other home networking devices.
- They have a large footprint and it is interesting to see them in the camera space.  It appears though that their whole smarthome space is fairly cobbled together.  There are two brands that they seem to have, one that is in house and one that was purchased, and they have yet to combine them.  This actually causes much confusion in the community and causes frustrations as to what works with what as they have two different ecosystems
- Their cloud storage is entirely optional, and their cameras can have 512 GB microSD cards installed.
- ### Concerns
  - Their privacy policy is universal accross all their products and seems to be very aggressive when it comes to actual data collection
  - They provide AI assissted detections, which means that they are probably using footage stored in their cloud to train the AI.
### Documentation
- Manufacturer Information
  - https://www.tp-link.com/us/landing/security-commitment/
  - https://www.tp-link.com/us/press/security-advisory/
  - https://privacy.tp-link.com/web/official/privacy-policy?region=US
  - https://www.tapo.com/us/tapocare/
  - [Tapo and Kasa](https://www.reddit.com/r/TPLinkKasa/comments/15r26o5/tplink_kasa_or_tplink_tapo/?rdt=37372)
- Case Studies
  - https://www.diva-portal.org/smash/record.jsf?pid=diva2%3A1619459&dswid=8884
  - https://ieeexplore.ieee.org/abstract/document/9766814
  - Not Cameras but may be useful - https://dl.acm.org/doi/abs/10.1145/3282894.3289735