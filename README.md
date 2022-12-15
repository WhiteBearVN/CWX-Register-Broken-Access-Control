# CWX-Register-Broken-Access-Control

- Report: November 2022
- Affected: Tested on v8.5.6
- Fix: No information
- Credit: WhiteBearVN_

## Description
Temenos CWX has an Broken Access Control vulnerability in /Registration.aspx, leak serial number and can be updated information, welcome message at home page

### Steps to reproduce
1. User login, we will not see Registration page at the right top corner, because this function only show for Admin user

![Alt text](login.jpg?raw=true)

2. Access to /Registration.aspx page successfully 

![Alt text](Access.jpg?raw=true)

3. See serial number and update welcome message

![Alt text](information_and_update.jpg?raw=true)

### Expected result

- Should be display forbidden notification
