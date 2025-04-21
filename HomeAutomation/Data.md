# Home automation - Historical reference only

## Tuya/SmartLife switches and bulbs.  
- SmartBulbs and switches fall largely into the same device category as technically they are mostly the same.  The exception would be their are smart bulbs which contains a speaker/microphone, and they would be included under Entertainment->Speakers.  
- Tuya is the parent company, which provides a  [SaaS and device certification program](https://www.tuya.com/platform/vas/works-with) for hardware manufacturers.  They also market their own devices under the SmartLife name.  
- While I selected Tuya, Expressif operates as a competitor with the RainMaker Sass offering under the same name.  They market towards higher value devices, like appliances and will be covered in that section.
- ### Concerns
   - Consumers don't really know what they are buying with 100s of different vendors all selling the same basic devices under different names.
   - There are different versions of Tuya's backend over the years, with some improvement in new versions, but many older devices are still manufactured and marketted.  Different devices use different back ends within the same app.
   - Tuya is the [world's leading](https://www.atlantis-press.com/proceedings/icssed-22/125973899) smart home company and very little has been written about their security, however there is plenty about the company as a whole.
   - Anyone can manufacture a SmartLife device and get it certified that does anything they want.  Tuya enforces only standards of operability, not functionality.
   - Numerous CVE's - [Example: CVE-2024-3764 Detail](https://nvd.nist.gov/vuln/detail/CVE-2024-3764)
   - Researchers have [urged the US government] (https://www.voanews.com/a/east-asia-pacific_voa-news-china_cybersecurity-experts-worried-chinese-firms-control-smart-devices/6209815.html) to ban Tuya devices over privacy concerns.
 - ### Refences
   - [Tuya Privacy Policy](https://images.tuyacn.com/app/smart/Privacy_Policy_en.html) with a vague Information Safety Safeguards section.

## Govee Temperature and Other sensors (water, weather, etc.)
- GoveeLife operates a similiar Saas service to Tuya/SmartLife, but they don't sell this service.  They offer different products under different iterations of the Govee name, GoveeLife/Home/SmartLife (confusing), etc.  
- Low power temp sensors are typically BlueTooth, and connect to a WiFi gateway.  However they can operate with just the Govee application and Bluetooth, eliminating the cloud requirement, but they require cloud for setup.  This limits features, and data retention.
- Govee is unique in offering a published, but poorly documented [API](https://developer.govee.com/docs/getting-started).
- ### Concerns  
  - The GoveeLife app requires location permissions, which is used for proximately controls of lights.  However like many apps, this is a global setting, so even if I only have temp sensors, I still have to give this permission.
  - Govee devices [do not use encryption](https://community.home-assistant.io/t/security-concerns-with-govee-devices-seeking-solutions-and-alternatives-h5072-h5075/683314/2), and instead Govee has implemented a device safety feature.  This features, which is not enabled by default means that once a Govee device has connected to one installation of the app, it can only connect to that copy of the running app.  This prevents other control devices on your network from connecting to it, but does not prevent network sniffing of the plain text data.  This is a strange work-around for not using encryption - likely related to the low compute power of the sensors and gateway.  The Govee API gateway however does require SSL.
  - Govee devices are [considered to be rather chatty](https://hal.science/hal-04936304/), despite not being ask to do anything.  
   - [Govee CVE - CVE-2023-3612](https://nvd.nist.gov/vuln/detail/CVE-2023-3612)  

- ### References
   - [Govee Privacy Policy](https://us.govee.com/pages/privacy-policy?srsltid=AfmBOoos77IPMaQoDdTlP_Xt3Wt2d-gZVVijfFM5jtmRVmissv2iA5hi) which is very minimal compared to Tuya.

## Utec/UHome/ULTRALOQ Locks
- Several different models of locks are offered.  Local options include fingerprint, pin pad, BlueTooth, and NFC.  All offer, and require cloud for at least setup.  Some use a gateway, others offer native WiFi.
- Useful features include logging, temporary codes, code disable, etc.
- ### Concerns  
  - [This article, ](https://ieeexplore.ieee.org/abstract/document/9537052) focuses on the biometrics that many locks use, which are stored by the SaaS provider vs. the device in most cases, which does not eliminate the cloud requirement.  Most PIN pad devices do store PINs locally to eliminate the cloud requirement as a failsafe.
  - [Focus on consumer](https://dl.acm.org/doi/abs/10.1145/2897845.2897886)  vs. industrial access control systems.
  - Previous but addressed [CVEs](https://app.opencve.io/cve/?vendor=u-tec&product=ultraloq_ul3_bt) in Bluetooth personal area network (out of scope)
  - [Additional information](https://threatpost.com/smart-lock-turns-out-to-be-not-so-smart-or-secure/146091/) on CVE's since the CVE are now gone.
- ### References
[U-tec Privacy Policy](https://u-tec.com/pages/privacy-policy?srsltid=AfmBOoo0yIuD85ULq2vXDMGjVI0cX4OCeGmXthHwxZsetD_HnxAevtqy)

## Kidde Alarms  
- Kiddie is a well known manufacturer of traditional smoke, fire, and CO alarms.  They have recently began offering WiFi equipped 110 volt AC alarms, some of which can also do air quality monitoring.  These devices can function as traditional alarms with a siren/light, but using the app offer typical smart home integration.
- Kidde offers air quality monitoring as a paid subscription.  
- ### Concerns  
  - Kidde went their own way, with their app and ecosystem.  It is poorly designed and implemented. 
  - The subscription service is misleading, but due to a bug in the app, you can subscribe and cancel, and the service remains.
  - Kidde is doing US based support, for a device designed and manufactured in China which is an odd choice as they don't seem to know anything about how their system works.
  - The initial products were subject to false alarms and [recalled](https://www.kidde.com/home-safety/en/us/support/product-alerts/recall-kidde-trusense/), not because of their IoT alarms but basic traditional alarm functionality.
  - Kidde alarms have been the subject of my personal research (Josh) because if the lack of public information I can find on them, and the issues I have had with them.
- ### References
   - [Carrier Privacy Policy](https://www.kidde.com/home-safety/en/us/legal/privacy-notice/)
   - Kidde is part of KGS, a subsidiary of Carrier, and there are several privacy policies.  The most interesting thing to note in these in the sections on Global data.
   - [KGB Privacy Policy](https://www.kidde.com/home-safety/en/us/legal/privacy-notice/)
   - There are more I could include as it is not clear which version would apply since there are so many.

## EcoBee Thermostats  
- Thermostats are one of the most common smart home devices found in many homes, where no other smart home devices may be used.
- Ecobee thermostats require the Internet, they can operate in a failsafe mode only without it. 
- ### Concerns  
- EcoBee has [closed their public api](https://www.ecobee.com/en-us/developers/) to future development - need to look at the why.
- EcoBee has integrations and provides [flexible load management data](https://www.ecobee.com/en-us/utilities/) with select utility providers, providing usage statistics to the utilities and allowing the utility some control over your thermostat.  This also means you usage data is shared or sold as has been used in many [reports](https://www.sciencedirect.com/science/article/abs/pii/S0360132323006558)
- EcoBee has gradually removed more and more functionality from the thermostat, and placed it only within the app.
- EcoBee partners only with Amazon Alexa, likely because of Google's competing Nest thermostat.  There is limited Google Home integration.  But this means your EcoBee thermostat is also an Alexa Speaker (covered in another category)
 - EcoBee thermostats work by proximity sensing.  They know if you are home or now.
 https://ijitra.com/index.php/ijitra/article/view/48/39
 - [Numerous CVEs](https://app.opencve.io/cve/?vendor=ecobee).  One example includes default root credentials.
 - In personal expierence with Ecobee support, Ecobee is able to produce detailed run statistics for your device, as well as a list of operations performed by its Amazon Alexa interface.  The later was a surprise as I would have expected Amazon to have that API more secured.
 - ### References
    - Ecobee has an entire [site](https://www.ecobee.com/en-us/privacy-policy/) dedicated to privacy and security, which is not a surprise given that Ecobee has Amazon Alexa integrations and shares your data (opt in) with utilities.


## Shared Concerns  
- All apps require you to give them a WiFi password to connect the device to the Internet and Cloud.  Most devices remember this password within the app and SaaS application.  This is not unique to Home Automation however, but more common, because the devices themselves lack the ability to store anything except "state".
- Applications use an all or no permissions model.  Meaning that regardless of the permissions needed for the particular type of device you purchased (location, contacts, etc.), you have to grant the permissions to the app even if they are not required.  
- Lots of data, with lots of different, separate it is not overly useful.  Aggerated, it becomes very powerful.
- Lack of encrypted communication is still common.  Reverse engineering has been highly successful as shown in the Open Source [Home Assistant](https://www.home-assistant.io/) project. 
- There are concerns with any [home automation ecosystem](https://www.journals.gaftim.com/index.php/ijcim/article/view/34/22); Alexa, GoogleHome, Home Assistant, etc.
- While enthusiast in  Home Automation community have embraced security and non-cloud requirements, this comes largely from the original non-cloud technologies like Zigbee.  Google's [Matter](https://jasondeegan.com/this-google-home-update-is-poised-to-revolutionize-home-automation/) has brought a renewed interest in non cloud home automation, but there are very few devices available.  Cheaper, simple cloud devices sell better and that is all the average consumer wants. 
