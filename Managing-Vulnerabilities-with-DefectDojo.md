# Finding Page of DefectDojo

## Overview
DefectDojo is a comprehensive DevSecOps platform designed to help organizations manage and streamline their application security programs. The Findings page is a critical component of DefectDojo, where security professionals can manage, analyze, and act upon vulnerabilities discovered during security assessments. This documentation provides an overview of the key features and functionalities of the Findings page, enabling users to efficiently navigate and utilize this essential part of the platform.

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


## Key Features of the Findings Page

### 1. Severity
  * The Severity column indicates the level of risk associated with each vulnerability, categorized into levels such as Low, Medium, High, and 
         Critical.   
  * Helps prioritize vulnerabilities based on their potential impact on the application or system.

###  2. Name
  * The Name column displays a brief description of the vulnerability, often reflecting the type of issue or the affected component.
 * Provides a quick understanding of the nature of the vulnerability, aiding in the rapid assessment of the findings.

### 3. CWE (Common Weakness Enumeration)
  * CWE is a standardized list of common software security weaknesses. Each vulnerability is assigned a CWE ID that categorizes the type of weakness.
 * Allows for standardized tracking and referencing of vulnerabilities, facilitating better communication and documentation.

### 4. Vulnerability ID
   * A unique identifier assigned to each vulnerability within DefectDojo. This ID is used internally for tracking and managing vulnerabilities.
   * Provides a unique reference for each finding, ensuring that vulnerabilities can be easily located and referenced across the system.

### 5. EPSS Score (Exploit Prediction Scoring System)
   * The EPSS Score represents the likelihood that a vulnerability will be exploited in the wild. It is derived from the EPSS model, which uses 
          machine learning and historical data to estimate risk.
   * Assists in determining the urgency of addressing a vulnerability based on its potential to be exploited.

### 6. EPSS Percentile
   * The EPSS Percentile indicates the ranking of the vulnerability’s exploitability compared to other vulnerabilities. A higher percentile suggests 
         a greater likelihood of exploitation.
  * Provides additional context for prioritizing vulnerabilities based on their relative risk compared to other known issues.

### 7. Date
  * The Date column records when the vulnerability was first reported or discovered.
   * Helps track the timeline of vulnerability discovery, which is essential for managing SLAs and understanding the aging of issues.

### 8. Age
   * Age indicates the number of days since the vulnerability was reported. It is calculated by subtracting the discovery date from the current date.
  * Enables quick assessment of how long a vulnerability has remained open, helping to prioritize older issues that may require more immediate attention.

### 9. SLA (Service Level Agreement)
   * The SLA column tracks the time frame within which a vulnerability should be resolved according to predefined service level agreements.
   * Ensures that vulnerabilities are addressed within an acceptable time frame, helping organizations meet their security obligations and minimize risk.

### 10. Reporter
   * This field indicates the user who reported or discovered the vulnerability. Typically, it includes the username or a reference to the tool 
           that identified the issue.
   * Helps in tracking the source of the finding, which is useful for accountability and follow-up actions.

### 11. Found By
  * The Found By column identifies the tool or method used to discover the vulnerability, such as manual testing, automated scans, or third-party 
           integrations (e.g., Semgrep, Gitleaks).
 *  Provides context on the origin of the finding, aiding in the analysis of the tool’s effectiveness and guiding remediation efforts.

### 12. Status
  * The Status column reflects the current state of the vulnerability, such as Open, Active, Mitigated, or Verified.
  * Helps in tracking the progress of each vulnerability's resolution, ensuring that issues are actively managed and closed in a timely manner.
### 13. Group
 * Grouping is used to organize vulnerabilities under specific categories, products, or teams within the organization.
 * Enhances the management of vulnerabilities by allowing for the segmentation of findings based on relevant criteria, improving focus and 
          accountability.

### 14. Service
 * This field indicates the specific service or application affected by the vulnerability.
 * Provides detailed information about the impacted area, which is critical for targeted remediation efforts and risk assessment.

### 15.Bulk Edit Menu 
* When needing to update many findings with the same set of tags, the bulk edit menu can be used to ease the burden.
* Once a finding is selected, a new button appears with the name “Bulk Edit”. Clicking this button produces a dropdown menu with many options, but the focus is just on tags for now. Update the field to have the desired tag list as follows, and click submit

![Screenshot (1979)](https://github.com/user-attachments/assets/c83b086c-478b-452a-9c4c-200ae5d2b3ae)

## How DefectDojo handles duplicates
For example, let’s say that you had your Maximum Duplicates field set to ‘1’.
First, you import Test 1.  Your report contains a vulnerability which is recorded as Finding A.
Later, you import Test 2 contains the same vulnerability.  This will be recorded as Finding B, and Finding B will be marked as a duplicate of Finding A.
Later still, you import Test 3 which also contains that vulnerability.  This will be recorded as Finding C, which will be marked as a duplicate of Finding A.  At this time, Finding B will be deleted from DefectDojo as the threshold for maximum duplicates has been crossed.

![Screenshot (1983)](https://github.com/user-attachments/assets/8f07673f-2ad3-4124-8959-be67e0ee6fdc)



# User Instructions
## Navigating the Findings Page
## Login Procedure:
* Visit the DefectDojo demo server using the following URL: [DefectDojo dashboard](https://demo.defectdojo.org/dashboard).
* Enter the username: admin.
* Enter the password: 1Defectdojo@demo#appsec.
* Click on Login to access the platform.

## Accessing the Findings Page:
* Once logged in, navigate to the main dashboard.
* Click on the "Findings" tab in the navigation menu to open the Findings Page.

## Using Filters and Sorting:
* Use the filter panel on the left to apply desired filters.
* Click on column headers to sort findings based on different attributes.
* Tags can be filtered in many ways through both the UI and the API. 

![Screenshot (1981)](https://github.com/user-attachments/assets/aae24584-2a35-4693-9fe9-2def77d54aef)


## Performing Actions:
* Select a finding to view detailed information.
* Use the action buttons to triage, resolve, or integrate findings with other tools.

## Create Findings
Any vulnerabilities which were not contained in the previous import will be added to the Test automatically as new Findings.



