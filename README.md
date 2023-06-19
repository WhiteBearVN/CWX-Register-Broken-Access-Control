# CWX Register Broken Access Control

- Report: November 2022
- Affected: Tested on v8.5.6
- Fix: No information
- Credit: WhiteBearVN_
- ID: CVE-2022-45287, CVE-2023-34797

## Description
Temenos CWX has an Broken Access Control vulnerability in /Registration.aspx, leak serial number and can be updated information, welcome message at home page

### Steps to reproduce
1. User login, we will not see Registration page at the right top corner, because this function only show for Admin user (CVE-2022-45287)

![Alt text](login.jpg?raw=true)

2. Access to /Registration.aspx page successfully and can be update welcome message, page info  

![Alt text](Access.jpg?raw=true)

3. Take the serial number and update the license (CVE-2023-34797)

![Alt text](information_and_update.jpg?raw=true)

### Expected result

- Should be display forbidden notification for all this functions
