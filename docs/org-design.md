# Design

## Groups
- There will be a group specifically made for **contractors** which will be based on MFA. Contractors can and will be placed in different departments (HR,IT,etc). Difference between an employee and contractor, in terms of policies, will be based on MFA. Northwind will not provide contractors with employee devices. Contractors will be required to authenticate via a code as well as password; all of which is directed by policies.

# Why each group exists
NWS - ATL - Dept - Finance
  - This group exists to provide a way to provide Finance department access to Quickbooks software. Software is to tally and manage expenses.
NWS - ATL - Dept - HR
  - This group exists to provide Human Resources department access to Workday. Workday is the application to manage employees.
NWS - ATL - Dept - IT
  - This group provides Information Technology department access to Splunk. Splunk is the monitoring and logging platform for the organization.
NWS - ATL - Dept - Sales
  - This group provides Sales department access to Salesforce. Salesforce is the organizations CRM (customer resources managemet) platform.
NWS - ATL - Role - Contractors
  - This role is specifically to provide access for contractors. This role applies stricter MFA policies as Contractors will not be provided company devices (phones).
NWS - ATL - Role - HelpDesk
  - This role is for HelpDesk. It provides them access to remote into employee devices if they need assistance. HelpDesk Technicians will still be under the IT department. 

# Where my model would start to strain
- It was important to group by department so that there is a clear and defined line between what each employee does and what each employee has access to. Groups allow the IT department to not have access to HR department applications. This model would start to strain with the addition of more roles that may be tied to multiple Departments.


## Users
# Employees
- There will be various users placed in multiple groups based on their specific role. Helpdesk is a **role**, however it is part of the IT **Department**. This is reason for a Helpdesk Tech to be in multiple groups. This reasoning also applies to contractors. There is no contractor department, but there will be contractors in various departments.

# Contractors
- 

## Tools
- CRM (Customer Resources Management) will be Salesforce
- HRM (Human Resources Management) will be Workday
- Security and monitoring tool will be Splunk
- Finances will be Quickbooks

