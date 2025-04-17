## [LG Smart Oven](LG-Oven-Analysis.md)


## [AEG Smart Oven](AEG-Oven-Analysis.md)


## [Samsung Smart Fridge](Samsung-Fridge-Analysis.md)


## [Beko Smart Fridge](Beko-Fridge-Analysis.md)

# Appliances

## Smart Fridge 
- Samsung Smart Refrigerator, since this is manufactered by a well known company it is interesting to see how often they are involved in vulnerability discussions.
- Beko Smart Fridge manufacturer'Arçelik' is one of the first companies to push the IASME IoT Security Assured certification for their connected refrigerator.
- Smart fridges should be included in this IoT Buyer’s Guide due to their security vulnerabilities. This includes risks like SSL misconfiguration and botnet attacks. They also pose privacy concerns, as they collect and store user data in the cloud. Many models depend on an always-on internet connection, which can cause issues if manufacturers discontinue cloud services.
- As with many IoT devices, limited security update lifecycles can leave devices vulnerable over time. As major point of the guide a lack of consumer awareness leads to poor security practices, which increases the risk of cyber threats.
- ### Concerns
   - Smart refrigerators have been identified as potential targets for cyberattacks. For instance, vulnerabilities in certain models have allowed unauthorized access, leading to concerns about data breaches and unauthorized control. 
   - Access to smart fridge technology controlled by IoS and Android apps could lead to unauthorized access. Many devices are shipped with default usernames and passwords, which users often neglect to change, making them susceptible to unauthorized access.
   - Some appliances transmit data without encryption, allowing attackers to intercept sensitive information.
- ### Case Studies
   - In 2014, a large-scale cyberattack leveraged over 100,000 smart devices, including refrigerators, to form a botnet. This network was used to send approximately 750,000 malicious emails over a two-week period. The incident highlighted the potential risks associated with unsecured IoT appliances and the ease with which they can be exploited for malicious purposes. https://www.mcafee.com/blogs/mobile-security/internet-of-things-cyberattack/
   - Research conducted by VTO Labs revealed that smart refrigerators could store extensive information about their owners. This data retention poses privacy risks, as unauthorized access to the appliance could lead to the exposure of sensitive personal information. The findings underscore the need for robust security measures to protect consumer data in IoT devices. https://www.technologyreview.com/2023/05/08/1072708/hack-smart-fridge-digital-forensics/
- ### Security
   - SSL Certificate Validation Issue: Samsung's RF28HMELBSR smart refrigerator was found to improperly validate SSL certificates, making it susceptible to man-in-the-middle attacks and exposing user credentials. ​https://blog.checkpoint.com/security/oems-have-flaws-too-exposing-two-new-lg-vulnerabilities/
   - Regarding Beko smart refrigerators, there are no publicly documented CVEs specific to their models at this time. However, it's essential for consumers to remain vigilant and ensure all smart appliances are regularly updated to mitigate potential security risks.​

## Smart Ovens
- Smart ovens integrate internet connectivity to offer features like remote monitoring and recipe downloads. However, these conveniences come with potential security risks that consumers should be aware of.
- LG Smart Ovens have been shown to have security vulnerabilities in its smart ovens, that show the importance of robust security measures. ​
- AEG Smart Ovens have had reports that indicate certain smart ovens perform frequent internet connectivity checks, raising concerns about data privacy and security practices.
- As with many IoT devices, limited security update lifecycles can leave devices vulnerable over time. As major point of the guide a lack of consumer awareness leads to poor security practices, which increases the risk of cyber threats.
- ### Concerns
   - Some of the major security and privacy risks identified in smart ovens face threats like unauthorized remote access, unencrypted data transmission, and weak security protocols, which can expose user data to cyberattacks. 
   - Many smart ovens require continuous internet connectivity for full functionality, and manufacturers may fail to provide long-term security updates, leaving devices vulnerable over time. This is a well documented problem among IoT devices with internet dependency and update limitations.
   - Users often neglect essential security measures, such as changing default passwords, updating firmware, and disabling unnecessary cloud features, increasing the risk of exploitation. This will benefit from Consumer Awareness & Best Practices that could be included in the guide based on IoT compliance requirements like NIST Cybersecurity Framework, ISO/IEC 27001, ISO/IEC 27032, and the OWASP IoT Security Verification Standard.
- ### Case Studies
   - A vulnerability in LG smart home devices allowed hackers to remotely control ovens, posing serious safety hazards. Unauthorized users could turn ovens on or off, increasing the risk of fires or accidents, highlighting major security flaws in IoT appliances. https://www.securityweek.com/security-flaw-could-have-let-hackers-turn-smart-ovens/
   - AEG smart ovens were discovered to frequently ping various websites, even when not necessary, raising privacy concerns about potential data exposure. These constant network queries could make user data vulnerable to interception and cyberattacks, emphasizing risks related to unnecessary smart appliance communication.
 https://hackaday.com/2023/02/03/smart-ovens-are-doing-dumb-checks-for-internet-connectivity/
- ### Security
   - 
 
## Shared Concerns
- Many IoT appliances have short update cycles, this leaves the devices vulnerable over time. Buyers should choose brands that commit to long-term security updates and avoid devices without clear patch policies. This is something that buyers should be aware of and companies should be committed to expressing for long-term and repeat consumers. 
- Some smart fridges and ovens require constant cloud connectivity, like many IoT devices, and they could lose critical features or stop working if the manufacturer discontinues support. Buyers should check if essential functions work offline before purchasing, or companies should be required to express with a rating system or symbol of compliance with this requirement.
- These appliances that collect and transmit user data, are sometimes communicating without encryption or user control opt-in. Buyers should seek out security certifications such as IASME IoT Security Assured and disable unnecessary cloud features to limit data exposure. Companies should also be required to allow users to opt-in to this type of data collection. 
- Many users neglect to update firmware or change default passwords, making their devices easy targets for hackers. Buyers should regularly update their devices, change default credentials, and follow manufacturer security guidelines to protect their privacy and security. If companies and manufacturers are unable or unwilling to provide this documentation and instruction there should be a rating system similar to the FTC that makes consumers aware.


