# Basic Employee Onboarding (AD)(RBAC)

## Problem Statement

Northstar Medical Group lacked a structured Active Directory environment for managing employee accounts and access. User accounts were not consistently organized by department, and permissions depended on manual processes instead of standardized security groups. This created administrative inefficiencies, incorrect access assignments, and potential HIPAA security risks. A centralized and role-based identity management structure was required.

## Solution Overview

I built a new Active Directory domain named NMG.com and configured NMG-DC01 as the domain controller. I created separate organizational units for Finance, Human Resources, Information Technology, and Operations. Global security groups were created for every department to implement role-based access control. Fifteen employee accounts were provisioned with standardized usernames, UPNs, departments, job titles, and group assignments. I also investigated and resolved incident NMG-0047 by moving Jane Cooper into the correct HR OU and correcting her security-group membership.

## Video Walkthrough

Video walkthrough link: Coming soon.

A video demonstration of the lab environment will be recorded and added during the next phase of the project.

## Tools Used

* Windows Server
* Active Directory Domain Services
* Oracle VirtualBox
* UTM
* Role-Based Access Control (RBAC)
* GitHub
* Group Policy

## Project Timeline

* Day 1: Domain creation and domain controller promotion
* Day 2: Organizational unit and security group design
* Day 3: User provisioning and RBAC implementation
* Day 4: Incident response and resolution (NMG-0047)
* Day 5: Documentation and case study packaging

## Key Accomplishments

* Built the NMG.com Active Directory domain from scratch
* Created four departmental organizational units
* Created four Global Security groups
* Provisioned and documented 15 employee accounts
* Implemented department-based RBAC
* Identified and corrected an incorrectly placed user account
* Corrected improper security-group membership
* Documented the investigation and resolution of ticket NMG-0047
* Organized technical documentation and screenshots in GitHub

## Repository Structure

* `Documentation/` — Domain configuration, security-group documentation, user list, and RBAC structure
* `Screenshots/` — Evidence from the Active Directory implementation
* `Incident-Reports/` — Incident investigation and resolution documentation

## Security Considerations

This project follows the principle of least privilege by assigning access through departmental security groups. User accounts receive permissions according to their job responsibilities and department. Proper OU placement also ensures that the correct policies can be applied to each employee.
