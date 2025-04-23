## [Tuya/SmartLife switches and bulbs](Tuya-Analysis.md)
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | Yes | There is no local communication option past setup.   |
| Requires Constant Connection to Company Cloud Infrastructure | Yes | All control is via API calls to the cloud service.   |
| Data Storage Requirements | Cloud | You can not opt out of usage collection, even if you are not using it the features that require it.   |
| Data Gathering Risk Score | 4 | The data that is gathered is not sensitive, but this is the nature of the product. |
| Company Vulnerability Remediation Score | 1 | They seem to have remediated issues via new products vs. patching or updating firmware on existing products as evidence by the various backends.|
| Company Vulnerability Transparency Score | 1 | Tuya has never disclosed vulnerabilities in products. | 

<sub> [Tuya SaaS Platform](https://www.atlantis-press.com/proceedings/icssed-22/125973899)</sub>    
<sub> [World's Leading Supplier of smart home devices](https://www.tuya.com/platform/vas/works-with)</sub>  
<sub> [CVE-2024-3764](https://nvd.nist.gov/vuln/detail/CVE-2024-3764)</sub>  
<sub> [Concerns of Chinese SaaS Cloud Platorms](https://www.voanews.com/a/east-asia-pacific_voa-news-china_cybersecurity-experts-worried-chinese-firms-control-smart-devices/6209815.html)  </sub>  
<sub> [Privacy Policy](https://images.tuyacn.com/app/smart/Privacy_Policy_en.html)</sub>  

## [Govee Temperature and Other sensors (water, weather, etc.)](Govee-Analysis.md)
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | No | While local connectivity is an option after intial setup, most users would not chose this option as it is not the default. |
| Requires Constant Connection to Company Cloud Infrastructure | No | As noted above, for most users this would be a yes.  While the device can be used with just Bluetooth, strange app behavior can occur as this is not the expected configuration. |
| Data Storage Requirements | Cloud | It is not entirely clear how much data is stored locally vs. cloud, and how it is synched.  This is likely do to the Bluetooth connection alternative.  They claim to only store 12 months of data, but it has been reported that it is stored longer.  Testing of this statement will be complete May 1st.  |
| Data Gathering Risk Score | 4 | The device's purpose is to collect data, and because of the hardware, it only collects the data it has disclosed. |
| Company Vulnerability Remediation Score | 1 | Like Tuya, Govee has not disclosed vulnerabilities of addressed them and instead focused on new products. |
| Company Vulnerability Transparency Score | 1 | Govee has never disclosed vulnerabilities in products. | 

<sub> [Encrytption vs. Non-Encryted Traffic](https://community.home-assistant.io/t/security-concerns-with-govee-devices-seeking-solutions-and-alternatives-h5072-h5075/683314/2) </sub>  
<sub> [API Documentation](https://developer.govee.com/docs/getting-started) </sub>  
<sub> [Chatty analysis](https://hal.science/hal-04936304/) </sub>  
<sub> [CVE-2023-3612](https://nvd.nist.gov/vuln/detail/CVE-2023-3612) </sub>   
<sub> [Privacy Policy](https://us.govee.com/pages/privacy-policy?srsltid=AfmBOoos77IPMaQoDdTlP_Xt3Wt2d-gZVVijfFM5jtmRVmissv2iA5hi) </sub>  

## [U-tec/UHome/ULTRALOQ Locks](Utec-Analysis.md)
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | Yes | The lock can operate with limited functionality in Bluetooth only mode after intial setup.   |
| Requires Constant Connection to Company Cloud Infrastructure | Sometimes | For full functionality, the device requires Internet connectivity but can operate with limited functionality with Bluetooth only, or with no connectivity via other methods.  Or with PIN or biometric, and as a last resort physical key. |
| Data Storage Requirements | Cloud | Critical data is stored in the cloud and on the device.|
| Data Gathering Risk Score | 3 | Proximity data is optional.  Biometrics stored in the device vs. the Cloud was a wise choice. |
| Company Vulnerability Remediation Score | 3 | U-Tec has released fixes, but continues to ignore general inquiries. |
| Company Vulnerability Transparency Score | 3 | All disclosed vulnerabilities have been common to Bluetooth vs. specific vulnerabilities in the device of their systems. | 

<sub> [Local Storage of PINs and biomerics](https://ieeexplore.ieee.org/abstract/document/9537052) </sub>  
<sub> [Common Bluetooth CVEs](https://app.opencve.io/cve/?vendor=u-tec&product=ultraloq_ul3_bt) </sub>  
<sub> [Additional CVE references](https://threatpost.com/smart-lock-turns-out-to-be-not-so-smart-or-secure/146091/) </sub>  

## [Kidde Alarms](Kidde-Analysis.md)
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | No | Can be setup with no connection at all, with limited functionality. |
| Requires Constant Connection to Company Cloud Infrastructure | No | The device can function as a traditional and inter-connected alarm via standard 3 wire systems (interconnect).
| Data Storage Requirements | Cloud | Event data is stored in the Cloud, as well as air quality monitoring data. |
| Data Gathering Risk Score | 4 | Only the required data is collected. |
| Company Vulnerability Remediation Score | 4 | Kidde has addressed product issues, but not faced IoT issues yet. |
| Company Vulnerability Transparency Score | 3 | Given they have addressed product safety issues they score well.  But this product has not been on the market long enough for full IoT analysis.  It is not likely to score well at a later time as Kidde did their own IoT backend rather than use a common platform. | 

<sub> [Carrier Privacy Policy](https://www.kidde.com/home-safety/en/us/legal/privacy-notice/) </sub>   
<sub> [KGB Privacy](https://www.kidde.com/home-safety/en/us/legal/privacy-notice/)    </sub>  
<sub> [Product Recalls](https://www.kidde.com/home-safety/en/us/support/product-alerts/recall-kidde-trusense/) </sub>  

## [Ecobee Thermostats](Ecobee-Analysis.md)
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | No | Can function as a stand alone device |
| Requires Constant Connection to Company Cloud Infrastructure | No | Can still function as a stand alone thermostat. |
| Data Storage Requirements | Cloud | All data is stored in the Cloud. |
| Data Gathering Risk Score | 1 | A lot of data is collected on usage and proximity/presence.  It knows when you are home and active. |
| Company Vulnerability Remediation Score | 2 | Google purchased Nest back in 2014, and suffered a major breach of all customers 5 years later.  They appear to be on top of their security since then, but you cannot check their updates prior to 2022.   |
| Company Vulnerability Transparency Score | 1 | Govee closed their API rather than addressing issues with it. | 

<sub>[Ecobee Beestat data example](https://app.beestat.io/)</sub>  
<sub>[Flexible load management](https://www.ecobee.com/en-us/utilities/)</sub>  
<sub>[Beestat example](https://app.beestat.io/)</sub>  
<sub>[Proximaty sensing concerns](https://ijitra.com/index.php/ijitra/article/view/48/39)</sub>  
<sub>[CVE list](https://app.opencve.io/cve/?vendor=ecobee)</sub>    
<sub>[Closed API and end of Developer Progran](https://www.ecobee.com/en-us/developers/)</sub>  
