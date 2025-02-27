## Initial Information Gathering
1. Decide on the device that will be getting analyzed
2. Find manufacturer information
   - Company
     - Parent Company?
   - Country of origin
3. Platform/ecosystem
   - Does it use its own or a different companies
   - Is that platform hosted on a PaaS
4. Research Studies including this device.
   - Google Scholar or IEEE
   - Some other Database of case studies
5. Breach/Vulnerability Reports
   - CVSS database

## Analysis
1. Internet/Network Requirements
2. Cloud Requirements
3. Data Storage Requirements
4. Data Gathering
   - Terms of Service
   - Case Studies
   - General Research
5. Company Vulnerability Remediation
   - CVSS database
   - Public Disclosures
   - Time Frame Between when Vulnerability was disclosed and Patch deployed
6. Company Vulnerability Tansparency
   - Were patches silently deployed or publically shared
   - Were vulnerabilities disclosed publically and how did the company respond
   - Company bug bounty programs

## Scoring
The higher the score the better

1. Place scores in the matrix  
    ## Example
    ### Camera X
    | Category | Score | Reasoning/Sources |
    | :------: | :---: | :-------: |
    | Requires Constant Internet Connection | Yes | Reasoning |
    | Requires Constant Connection to Company Cloud Infrastructure | No | Reasoning |
    | Data Storage Risk Score | Hybrid | Reasoning |
    | Data Gathering Risk Score | 3 | Reasoning |
    | Company Vulnerability Remediation Score | 2 | Reasoning |
    | Company Vulnerability Transparency Score | 4 | Reasoning |

2. Provide a total scoring at the bottom of the matrix
3. Give a summary describing the product, the manufacturer, platform, and reasoning for the score.
4. Give final recommendations