# Ticket: Grant Access to Finance Shared Folder (Access Request)

## Symptoms / Request
User requested access to the Finance shared folder to complete monthly reporting tasks.  
User receives “Access Denied” when attempting to open the folder.

## Ticket Type
Access Request

## Verification Steps
1. Confirmed user identity via Teams chat.  
2. Verified business need for access.  
3. Contacted Finance manager to approve access.  
4. Checked existing group membership in Active Directory.

## Troubleshooting Steps
1. Opened Active Directory Users and Computers (ADUC).  
2. Navigated to the **Security Groups** for Finance.  
3. Located the correct group: `FIN-Folder-Access`.  
4. Added the user to the group.  
5. Forced a permissions sync using `gpupdate /force`.  
6. Asked user to log out and back in to refresh token.  
7. Tested access with the user.

## Resolution
User successfully accessed the Finance shared folder after being added to the correct AD security group.  
No further issues reported.

## Root Cause
User was not a member of the required Finance security group.

## Skills Demonstrated
- Active Directory group management  
- Permission troubleshooting  
- Access control and security  
- User communication  
- Documentation and workflow handling
