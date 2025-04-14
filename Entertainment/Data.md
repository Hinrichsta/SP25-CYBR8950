# Entertainment


IoT has become a key part of entertainment, with gaming consoles like PlayStation, Xbox, and Switch relying on internet connectivity for cloud saves and online play. Streaming devices such as Roku, Chromecast, and Fire Stick provide easy access to digital content but raise concerns about data security. Smart speakers like Alexa and Google Nest enhance convenience but continuously listen, posing privacy risks. Even children's toys, like VTech products, now connect online, introducing potential security vulnerabilities.


## Sony, [Playstation 5](https://www.playstation.com/en-us/ps5/?smcid=pdc%3Aen-us%3Aps5-games%3Aprimary%20nav%3Amsg-ps5%3Aps5) & Playstation Network
- Sony is one of the biggest entertainment and gaming companies in the world, and PlayStation is one of the leading gaming platforms on the market. This also means they have extensive data collection and online services integrated into their ecosystem.
- All of their data is stored on Sony’s proprietary cloud platform and is developed to run within their PlayStation Network (PSN) system.
- They are generally consistent with releasing security patches and updates for their consoles and online services.
- ### Concerns
   - Sony collects a significant amount of user data, including gameplay activity, purchases, and interactions on PSN.
   - A PlayStation account and internet connection are required for many features, including online multiplayer and cloud saves.
   - Sony has faced past security breaches, including major incidents affecting PSN.
### Documentation
- Manufacturer Information
  - https://www.playstation.com/en-us/privacy-security-safety/
  - https://www.playstation.com/en-us/legal/privacy-policy/
  - https://www.playstation.com/en-us/legal/psn-terms-of-service/
- Case Studies
  - [Cloud Data Breach Disclosures: the Consumer and their Personally Identifiable Information (PII)](https://ieeexplore-ieee-org.leo.lib.unomaha.edu/document/9532579)
  - [A cloud you can trust](https://ieeexplore-ieee-org.leo.lib.unomaha.edu/document/6085778)

### Security
#### Disclosures
  - SECURE@SONY
    - https://hackerone.com/sony
    - https://hackerone.com/playstation
    - Disclosures
      - April 2011 – PlayStation Network Data Breach
        - One of the largest data breaches in gaming history, exposing 77 million accounts. The breach resulted in PSN being taken offline for nearly a month.
      - November 2022 – PlayStation 5 Kernel Exploit (CVE-2022-3349)
        - A kernel vulnerability allowing unauthorized code execution was disclosed by a security researcher. Sony issued a patch shortly after.
      - September 2023 – PlayStation Network API Exposure
        - A researcher identified a flaw that could allow unauthorized access to certain PSN account details, later patched by Sony.
      - December 2023 – PlayStation 5 Firmware Exploit (CVE-2022-33917)
        - Security researchers discovered a new exploit in the firmware allowing privilege escalation, leading to homebrew execution. Sony released a security update.
      - March 2024 – PlayStation Network Phishing Campaign
        - Users reported a widespread phishing campaign targeting PSN accounts, attempting to steal credentials and payment information. Sony advised users to enable 2FA and be cautious of phishing attempts.
    - Breaches
      - 2011 – PlayStation Network Data Breach
        - One of the largest gaming-related breaches, affecting 77 million users. Data including names, addresses, email accounts, and credit card details were compromised.
      - 2014 – Sony Pictures Hack
        - While not directly related to PlayStation, this attack by a hacker group resulted in the leak of sensitive Sony corporate data, emails, and unreleased films.
      - 2023 – Sony Alleged Ransomware Attack
        - Reports surfaced of a ransomware group claiming to have breached Sony and exfiltrated a significant amount of data. Sony did not confirm the full extent of the breach.
    - Notes
      - Sony maintains a Bug Bounty / HackerOne program for both playstation and related services
      - Users are strongly advised to enable two-factor authentication (2FA) on their PlayStation accounts.
      - Sony does not always publicly disclose all security vulnerabilities, but they consistently release patches and firmware updates.

## [Roku](https://www.roku.com/what-is-roku) Television
- Roku is a leading brand in smart TVs and streaming devices, offering access to thousands of apps and channels. Their platform integrates online services, including content recommendations, ads, and data collection.
- User data, such as preferences and viewing history, is stored on Roku’s cloud platform and linked to Roku accounts.
- They regularly release software updates for security and performance improvements.
- ### Concerns
   - Roku collects significant user data, including viewing habits, app usage, device information, and advertising interactions. This data is used for targeted ads and content recommendations.
   - Consumer Reports found that some Roku TVs were susceptible to remote access exploits, allowing attackers to control TVs over the network. Roku addressed the issue with a security update. [(2018 CVE Vulnerability Details)](https://www.cvedetails.com/cve/CVE-2018-11314/)
   - Roku has been criticized for sharing user data with third-party advertisers. In 2023, a lawsuit alleged that Roku failed to properly protect user data, leading to privacy concerns about data sales and tracking.
   - A Roku account and an internet connection are required for full functionality, including access to streaming services and software updates.
### Documentation
- Manufacturer Information
  - https://docs.roku.com/published/userprivacypolicy
  - https://docs.roku.com/published/deviceplayereula
  - https://docs.roku.com/published/deviceplayereula
    - [The Roku Channel Terms of Use](https://docs.roku.com/published/therokuchannel-userstermsandconditions)
    - [Protecting your Roku account](https://www.roku.com/blog/protecting-your-roku-account?srsltid=AfmBOorvJW5GU8DqZHgsEzlm63RDcyCyXjyOBSK3z8fLMA4OxxByQRau)    
- Case Studies
   - [RokuControl-Conducting MITM Attacks on Roku](https://ieeexplore-ieee-org.leo.lib.unomaha.edu/document/9946502)
   - [SoK: Security Evaluation of Home-Based IoT Deployments](https://ieeexplore-ieee-org.leo.lib.unomaha.edu/document/8835392)
   - [Security Properties of Virtual Remotes and SPOOKing their
violations](https://dl.acm.org/doi/abs/10.1145/3579856.3582834)
     - read section 2.2.3 of this [document](https://dl.acm.org/doi/pdf/10.1145/3579856.3582834) 

### Security
#### Disclosures



## [Amazon Alexa](https://www.amazon.com/Meet-the-new-Alexa/dp/B0DCCNHWV5)
- Amazon is one of the largest technology companies, and Alexa is a leading voice assistant platform, integrated into smart speakers, displays, and various IoT devices. This also means Amazon collects extensive user data to improve services and enable personalized experiences.
- All data is stored on Amazon’s cloud infrastructure and processed within their Alexa ecosystem.
- Amazon regularly releases updates to improve security, privacy controls, and functionality.
- ### Concerns
   - Amazon collects significant user data, including voice recordings, smart home interactions, and usage patterns.
   - Alexa devices require an Amazon account and an internet connection for full functionality.
   - Past privacy concerns include reports of human reviewers analyzing voice recordings and security flaws exposing user data.
### Documentation
- Manufacturer Information
  - [Alexa+ Trust & Privacy](https://www.amazon.com/b?node=203453976011&ref=dp_btf_xaa_spp_d_p5)
    - [Security Layers](https://www.amazon.com/b/?node=23638098011&ref=aucc_en_us_web_dom_xaa_evgn_tx_0016)
    - [Alexa Privacy (may not be accessilbe without acccount)](https://www.amazon.com/alexa-privacy/apd/home?ref=aucc_en_us_web_dom_xaa_evgn_tx_0021)
  - [Amazon Vulnerability Research Program (VRP)](https://hackerone.com/amazonvrp?type=team)
  - [Amazon Echo Software Security Updates](https://www.amazon.com/gp/help/customer/display.html?nodeId=GMZQWNQRVENX4GTQ)
- Case Studies
  - [Alexa, Are You Listening?: Privacy Perceptions, Concerns and Privacy-seeking Behaviors with Smart Speakers](https://dl.acm.org/doi/abs/10.1145/3274371)
  - [Alexa, is the skill always safe? Uncover Lenient Skill Vetting Process and Protect User Privacy at Run Time](https://ieeexplore-ieee-org.leo.lib.unomaha.edu/document/10554785)
  - [A Survey on Amazon Alexa Attack Surfaces](https://ieeexplore-ieee-org.leo.lib.unomaha.edu/document/9369553)
  - [Alexa Skills: Security Vulnerabilities and Countermeasures](https://ieeexplore-ieee-org.leo.lib.unomaha.edu/document/10066153)

## [Vtech](https://www.vtechkids.com/) Toys 
- VTech is a major manufacturer of electronic learning toys, offering smart devices designed for children. Their products often include internet connectivity, cloud storage, and interactive features, which also means they collect and process user data.
- All data is stored on VTech’s cloud platform "VTech Cloud" and linked to user accounts, primarily through services like Kid Connect.
- VTech provides software updates to improve security and functionality.
- ### Concerns
   - VTech collects personal data, including children's names, birthdates, and voice recordings.
   - Many features require an account and internet connection.
   - In 2015, VTech suffered a major data breach, exposing the personal information of over 6 million children and parents.
### Documentation
- Manufacturer Information
  - [Privacy Policy](https://www.vtechda.com/legal/version/view.aspx?country=US&lang=eng&x=4&y=1)
  - [Recall Information](https://www.vtechkids.com/recall)
- Case Studies
  - [The Internet of Toys](https://www.tandfonline.com/doi/abs/10.1080/22041451.2016.1266124)
  - [Pictures of Children' 'In Vtech Hack](https://www.bbc.com/news/technology-34971337)
  - [Electronic Toy Maker VTech Settles FTC Allegations That it Violated Children’s Privacy Law and the FTC Act](https://www.ftc.gov/news-events/news/press-releases/2018/01/electronic-toy-maker-vtech-settles-ftc-allegations-it-violated-childrens-privacy-law-ftc-act)
