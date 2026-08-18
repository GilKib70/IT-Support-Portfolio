# Ticket: Grant Access to Finance Shared Folder (Access Request with Escalation)

## Request
User requested access to the Finance shared folder to complete monthly reporting tasks.  
User receives “Access Denied” when attempting to open the folder.

## Ticket Type
Access Request (Escalation Required)

## Reason for Escalation
Finance shared folder contains confidential financial data.  
Access requires approval from the Finance Manager before permissions can be granted.

## Verification Steps
1. Confirmed user identity via Teams chat.  
2. Verified business need for access.  
3. Checked existing group membership in Active Directory.  
4. Confirmed user was not part of any Finance-related security groups.  
5. Escalated request to Finance Manager for approval.

## Escalation Details
- Sent approval request to Finance Manager via email/Teams.  
- Finance Manager confirmed user requires read-only access for reporting tasks.  
- Approval logged in the ticket.

## Troubleshooting / Implementation Steps
1. Opened **Active Directory Users and Computers (ADUC)**.  
2. Located the correct security group: `FIN-Folder-Access-ReadOnly`.  
3. Added the user to the group.  
4. Ran `gpupdate /force` to refresh permissions.  
5. Asked user to log out and back in to refresh token.  
6. Tested access with the user.

## Resolution
User successfully accessed the Finance shared folder after being added to the approved AD security group.  
No further issues reported.

## Root Cause
User was not a member of the required Finance security group.  
Access required managerial approval due to data sensitivity.

## Skills Demonstrated
- Active Directory group management  
- Permission troubleshooting  
- Escalation and approval workflow  
- Security and access control  
- Professional communication  
- Documentation and ticket handling
