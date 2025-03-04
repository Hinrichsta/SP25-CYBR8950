# Home automation

## Tuya/SmartLife switches and bulbs.  
- SmartBulbs and switches fall largely into the same device category.  The exception would be their are smart bulbs which contains a speaker/microphone, and they would be included under entertainment->speakers.  
- Tuya is the parent company, which provides a a [SaaS and device certification program](https://www.tuya.com/platform/vas/works-with) for hardware manufacturers.  They also market their own devices under the SmartLife name.  
- ### Concerns
   - Consumers don't really know what they are buying with 100s of different vendors all selling the same basic devices.  

## Govee Temperature and other sensors
- GoveeLife operates a similiar Saas service to Tuya/SmartLife, but they don't sell this service.  They offer different products under different iterations of the Govee name, GoveeLife/Home/SmartLife (confusing), etc.  
- Low power temp sensors are typically BlueTooth, and connect to a WiFi gateway.  However they can operate with just the Govee application and Bluetooth, eliminating the cloud requirement, but they require cloud for setup.  This limits features, and data retention.
- Govee is unique in offering a published, but poorly documented [API](https://developer.govee.com/docs/getting-started).
- ### Concerns  
  - The GoveeLife app requires location permissions, which is used for proximately controls of lights.  However like many apps, this is a global setting, so even if I only have temp sensors, I still have to give this permission.
  - Govee devices [do not use encryption](https://community.home-assistant.io/t/security-concerns-with-govee-devices-seeking-solutions-and-alternatives-h5072-h5075/683314/2), and instead Govee has implemented a device safety feature.  This features, which is not enabled by default means that once a Govee device has connected to one installation of the app, it can only connect to that copy of the running app.  This prevents other control devices on your network from connecting to it, but does not prevent network sniffing of the plain text data.  This is a strange work-around for not using encryption - likely related to the low compute power of the sensors and gateway.  The Govee API gateway however does require SSL.

## Utec/UHome/ULTRALOQ Locks
- Several different models of locks are offered.Local options unclude fingerprint, pin pad, BlueTooth, and NFC.  All offer, and require cloud for at least setup.  Some use a gateway, others offer native WiFi.
- Useful features include logging, temporary codes, code disable, etc.
- ### Concerns  
  - Kidde went their own way, with their app and ecosystem.  It is poorly designed and implemented.   It is difficult to setup and use.

## Kidde Alarms  
- Kiddie is a well known manufacturer of traditional smoke, fire, and CO alarms.  They have recently begun offering WiFi equiped 110 volt AC alarms, some of which can also do air quality monitoring.  These devices can function as traditional alarms with a siren, but using the app offer typical smart home integration.
- Kidde offers air quality monitoring as a paid subscription.  
- ### Concerns  
  - Kidde went their own way, with their app and ecosystem.  It is poorly designed and implemented. 
  - The subscription service is misleading, but due to a bug in the app, you can subscribe and cancel, and the service remains.

## EcoBee Thermostats  
- Thermostats are one of the most common smart home devices found in many homes, where no other smart home devices may be used
- Ecobee thermostats require the Internet, they can operate in a failsafe mode only without it. 
- ### Concerns  
- Ecobee has [closed their public api](https://www.ecobee.com/en-us/developers/) to future development - need to look at the why.
- Ecobee has integrations and provides [flexible load management](https://www.ecobee.com/en-us/utilities/) with select utility providers, providing usage statistics to the utilities and allowing the utility some control over your thermostat
- Ecobee has gradually removed more and more functionality from the thermostat, and placed it only within the app.
- Ecobee partners only with Amazon Alexa, likely because of Google's competing Nest thermostat.  There is limited Google Home integration.  But this means you Ecobee thermostat is also an Alexa Speaker (covered in another category)


## Shared Concerns  
- All apps require you to give them a WiFi password to connect the device to the Internet and Cloud.  Most devices remember this password with the app and SaaS application.  
- Applications use an all or no permissions model.  Meaning that regardless of the permissions needed for the particular type of device you purchased (location, contacts, etc.), you have to grant the permissions to the app even if they are not required.  
