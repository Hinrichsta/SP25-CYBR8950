# Google Nest Cameras
## Analysis
- **Name**: Wyze
- **Manufacturer**: Wyze Labs Inc
- **Country of Origin**: US Owned Company | Manufactured in China
- **Platform**: Wyze App | Can be integrated with Google Assisstant, Amazon Alexa and IFTT for funtionality only
- **Internet Requirements**:
    - Requires internet connection to access all video
    - Requires connection to Wyze to access all videos
- **Authentication**
    - Wyze accounts are required to have MFA by default, but uses email unless another is setup
    - Homes can be shared, but a single account cannot be used for multiple homes
- **Data Transmission Security**
    - Cameras only communicate over Wireless
    - Cameras have individual transmission encryption keys using both Symmetrical and Aysmmetrical Encryption
- **Physical Security**
    - Utilize a MicroUSB port for power
    - MicroUSB slot is uncovered and can be seen and accessed easily
- **Storage**
    - MicroUSB can be used for Local Storage
      - This is required if you want to utilize the Free Tier of Cameras
    - Cloud Storage
      - Requires a subscription for any video storage
      - 3 Tiers of Storage
        - Cam Plus - 14 days, but can only have 3 cameras and requires a subscription for each camera
        - Cam Unlimited - 14 days
        - Cam Unlimited Pro - 60 days
- **Data Requirements**
    - 1-2 Mbps for Standard Definition/camera
    - 4-7 Mbps for High Definition/camera
- **Data Gathering**
  - Gathers data about users through the Wyze Products that they utilize
  - Gathers face data for facial recognition and training
    - Privacy Policy states that all data is deleted after 30 days
    - This is a non-consent for non-users.  If anybody is seen in their camera's their likeness is collected
  - Utilizes your data for targeted advertising on 3rd party platforms
    - Explicityl stated used by Wyze and not the 3rd part platforms
  - Data is only shared within the Wyze company, and not shared or sold except in the event of breaking the law
- **Vulnerability Remediation**
  - Company appears to be on a monthly patching cycle
  - Vulnerabilities are getting disclosed
    - This seems to be more recent in the last 3 years
    - 2 Vulnerabilites from 2019 were not added to the NIST database until 2022
      - Possible that this is an error on NIST's side as they do have vastly different numbers
    - Gap between 2019 and 2023, and then multiple vulnerabilities in 2024
      - This isn't an indicator, but it is something to look at.
  - There have been 3 major breaches, 2 in 2022 and 1 in 2023
    - There was an exposed database, and video files were publically exposed in 2022
    - While not a breach, this appears to be from negligence.  In 2023 all camera feeds were viewable by anybody on the app.
  - There is a bug bounty program that they have set up, but it does not appear to have any major movement since the original creation.  There have been payouts made in the last 4 months though.
- **Vulnerability Transparency**
  - Vulnerability patching does not appear to be indicated in Release Notes that are publically accessible
  - Vulnerability disclosure on NIST dated 7/19/2024 for camera v4 Pro
    - Release notes do not state any remediation in the indicated Firmware update
  - 4 Vulnerabilities disclosed in November of 2024
    - No Release Notes indicating patching

## Scoring rubric
| Device Score-Category |  Rating | Description of Ratings | 
| :---: | :---: | :---: | 
| Requires Constant Internet Connection | Yes | There is local storage but it cannot be viewed without using the Wyze app |
| Requires Constant Connection to Company Cloud Infrastructure | Yes | The only location that video can be viewed from is the Wyze app, or the browser web view if you have a subscription |
| Data Storage Requirements | Hybrid | Data can be stored locally, and required if you do not have a subscription.  With a subscription both can be achieved |
| Data Gathering Risk Score | 4 | Overall they only gather data from their products, and through their connections to third party.  They do not sell data in anyway and it is primarily used for internal information.  The Facial recognition data does NOT require consent from those being recorded, but all data is deleted after 30 days |
| Company Vulnerability Remediation Score | 2 | They did not start disclosing vulnerabilities until about 2022 when they had their first major breach.  Since then they have done better with disclosures and making sure that the information is shared.  Their bug bounty program while existent is lacking. |
| Company Vulnerability Transparency Score | 1 | They do not make any effort to put their vulnerability patches into their patch notes.  Instead they are put into a seperate location in their forums that is difficult to find.  It does appear that it is getting updated, but you wouldn't know it without regularly checking.  They also do not appear to have been disclosing anything before 2022 which is an issue to start. | 

### Total Score: 7