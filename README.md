# Lab-1-Directory-Foundation

# Design

## Groups
- There will be a group specifically made for **contractors** which will be based on MFA. Contractors can and will be placed in different departments (HR,IT,etc). Difference between an employee and contractor, in terms of policies, will be based on MFA. Northwind will not provide contractors with employee devices. Contractors will be required to authenticate via a code as well as password; all of which is directed by policies.
- NWS - ATL - Dept - HR
- NWS - ATL - Dept - IT
- NWS - ATL - Dept - Sales
- NWS - ATL - Dept - Finance
- NWS - ATL - Role - Contractors
- NWS - ATL - Role - HelpDesk

## Users
- There will be various users placed in multiple groups based on their specific role. Helpdesk is a **role**, however it is part of the IT **Department**. This is reason for a Helpdesk Tech to be in multiple groups. This reasoning also applies to contractors. There is no contractor department, but there will be contractors in various departments.

## Tools
- HRM (Human Resources Management) will be Workday
      - HR
- CRM (Customer Resources Management) will be Salesforce
      - Sales
- Security and monitoring tool will be Splunk
      - IT
- Finance will be Quickbooks
      - Finance
