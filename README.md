# Project Overview

Northwind Services is a 15-person company that has been running on shared logins and a spreadsheet of who has access to what. They are moving to Microsoft Entra ID and they have hired you to set the directory up properly the first time.

# Tools Used
- GitHub
- Microsoft Entra
- Excel

# What I Built
- Built an Identity and Access management design for an organization that is newly created. Organization includes multiples departments (IT, HR, Sales, etc.) that will have multiple employees as well as contractors. Architected the design to account not only for current outlook, but also in preparation for company scale in different states. IDP (identity provider) used was Microsoft Entra.
  
# Screenshots

# Security Lessons Learned
- Group based access is always the most efficient way of managing multiple employees in an ever growing company. It provides the ability to adjust permissions for a specific application to multiple employees instead of doing one by one. It terms of auditing, group based access turns a "deep dive" for a permission issue into a easy "few second" resolution.
- Contractors that are given the same access as an employee, need to be managed properly to keep access from being granted even after a contractor leaves. This is why it is important to have a contractor group designated to properly audit and keep a breach from occurring.
  
# Future Improvements
- Setup MFA for employees and contractors as a whole. Executives will have a different MFA as they will have access to much more than regular employees.
- Setup SSO for applications that employees have access to. Goal is to make things as seamless as possible for employees/users.
- Setup connector in order to export Entra audit-logs into a monitoring platform, perhaps like Splunk or Elasticsearch.
- Script automation with PowerShell.

## Groups
- There will be a group specifically made for **contractors** which will be based on MFA. Contractors can and will be placed in different departments (HR,IT,etc). Difference between an employee and contractor, in terms of policies, will be based on MFA. Northwind will not provide contractors with employee devices. Contractors will be required to authenticate via a code as well as password; all of which is directed by policies.
- NWS - ATL - Dept - HR
- NWS - ATL - Dept - IT
- NWS - ATL - Dept - Sales
- NWS - ATL - Dept - Finance
- NWS - ATL - Role - Contractors
- NWS - ATL - Role - HelpDesk

**Without groups, creating and providing a user access to 3 different applications takes 4 different steps. With groups only takes two steps.**
