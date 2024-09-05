# Finding Page of DefectDojo

## Overview
DefectDojo, a DevSecOps platform, has a significant influence on how organizations manage their app security programs. The Findings page is crucial in DefectDojo. Security experts use this page to monitor, investigate, and address vulnerabilities discovered during security assessments.The Finding page plays a key role in handling and monitoring security weak spots in your apps. It gives you a full picture of all detected issues helping you evaluate, sort, and tackle vulnerabilities .

##   Example of Findings:
* OpenSSL ‘ChangeCipherSpec’ MiTM Potential Vulnerability
* Web Application Potentially Vulnerable to Clickjacking
* Web Browser XSS Protection Not Enabled

## Accessing the Findings Page
  *  URL: https://demo.defectdojo.org/finding
  *  Login Credentials:
  *  Username: admin
  *  Password: 1Defectdojo@demo#appsec1. 

![Screenshot (1980)](https://github.com/user-attachments/assets/3d39c642-f1b2-4bed-9a81-62d9840cb5e2)



# Key Features of the Findings Page
## Severity
* The Severity column shows how risky each vulnerability is. It groups them into levels like Low, Medium, High, and Critical.
* This helps teams rank vulnerabilities based on how much they could affect the application or system.
## Name
* The Name column gives a short description of the vulnerability. It often tells you what kind of issue it is or what part it affects.
* This lets you grasp what the vulnerability is about helping you assess the findings fast.
## CWE (Common Weakness Enumeration)
* CWE is a standard list of common software security flaws. Each vulnerability gets a CWE ID that puts it in a category of weakness.
* Enables consistent tracking and referencing of vulnerabilities making communication and record-keeping easier.
## Vulnerability ID
* A unique code given to each vulnerability in DefectDojo. This ID is used inside the system to track and handle vulnerabilities.
* Offers a unique tag for each finding making sure vulnerabilities can be found and mentioned across the system.
## EPSS Score (Exploit Prediction Scoring System)
* The EPSS Score shows how likely a vulnerability will be used by attackers. It comes from the EPSS model, which uses smart software and past data to guess risk.
* Helps decide how to fix a vulnerability based on its chance of being used by attackers.
## EPSS Percentile
* The EPSS Percentile shows how a vulnerability's exploitability ranks against others. A higher percentile means it's more likely to be exploited.
* This gives more insight to help prioritize vulnerabilities based on their relative risk compared to other known issues.
##  Date
* The Date column shows when someone first reported or found the vulnerability.
* This helps track when vulnerabilities are discovered, which is key for managing SLAs and seeing how old issues are.
## Age
* Age shows how many days have passed since someone reported the vulnerability. You get this by subtracting the discovery date from today's date.
* This lets you see how long a vulnerability has been open, which helps prioritize older issues that might need faster action.
## SLA (Service Level Agreement)
* The SLA column keeps track of the timeframe to resolve a vulnerability based on agreed-upon service levels.
* This column makes sure vulnerabilities get fixed enough helping companies meet their security duties and lower risks.
## Reporter
* This field shows who found or reported the vulnerability. It includes a username or mentions the tool that spotted the issue.
* It helps track where the finding came from, which is useful to hold people accountable and take next steps.
## Found By
* The Found By column shows how the vulnerability was spotted, like through manual checks automatic scans, or tools from other companies (for example Semgrep Gitleaks).
* This info sheds light on where the finding came from helping to assess how well the tool works and steer efforts to fix the issue.
##    Status
* The Status column tells you where things stand with the vulnerability right now such as Open, Active, Mitigated, or Verified.
* This helps to keep tabs on how each vulnerability is being dealt with making sure issues are handled and wrapped up .
## Group
* Grouping is used to sort vulnerabilities into specific buckets, products, or teams within the company.
* Improves vulnerability management by grouping findings based on key factors, which helps sharpen focus and boost accountability.
## Service
* This field points out the specific service or app affected by the vulnerability.
* Gives in-depth details about the impacted area, which is key to target fixes and gauge risks.
## Bulk Edit Menu
* When you need to update lots of findings with the same set of tags, you can use the bulk edit menu to make it easier.
* After you pick a finding, a new button shows up called "Bulk Edit". When you click this button, you'll see a dropdown menu with many choices, but we're just looking at tags right now. Change the field to have the tag list you want then click submit.

![Screenshot (1979)](https://github.com/user-attachments/assets/c83b086c-478b-452a-9c4c-200ae5d2b3ae)

## How DefectDojo handles duplicates
For example, let’s say that you had your Maximum Duplicates field set to ‘1’.
First, you import Test 1.  Your report contains a vulnerability which is recorded as Finding A.
Later, you import Test 2 contains the same vulnerability.  This will be recorded as Finding B, and Finding B will be marked as a duplicate of Finding A.
Later still, you import Test 3 which also contains that vulnerability.  This will be recorded as Finding C, which will be marked as a duplicate of Finding A.  At this time, Finding B will be deleted from DefectDojo as the threshold for maximum duplicates has been crossed.

![Screenshot (1983)](https://github.com/user-attachments/assets/8f07673f-2ad3-4124-8959-be67e0ee6fdc)


# User Instructions
## How to Use the Findings Page
### How to Log In:
* Go to the DefectDojo demo server: [DefectDojo dashboard](https://demo.defectdojo.org/dashboard).
* Type in the username: admin.
* Type in the password: 1Defectdojo@demo#appsec.
* Hit Login to enter the platform.
### To access the Findings Page:
* After logging in, go to the main dashboard.
* Click the "Findings" tab in the menu to open the Findings Page.
### To use Filters and Sorting:
* Use the filter panel on the left to apply filters you want.
* Click on column headers to sort findings by different attributes.
* You can filter tags in many ways through both the UI and the API.

![Screenshot (1981)](https://github.com/user-attachments/assets/aae24584-2a35-4693-9fe9-2def77d54aef)
  
### Taking Action:
* Pick a finding to see detailed information.
* Use the action buttons to sort out, fix, or link findings with other tools.
### Add Findings
Any security weak spots not included in the previous import will be added to the Test as new Findings.




