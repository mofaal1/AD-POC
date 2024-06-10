# Active Directory Proof of Concept

## Objective
Created an Organizational Unit (OU) hierarchy in Active Directory and implemented a file system mirroring the OU structure. Managed access to shares and directories specific to each unit’s employees in accordance with the department’s needs and requirements.

## Skills Learned
- Active Directory management
- OU and group structure creation
- File system security implementation
- Group Policy application and management
- User and group management in AD

## Tools Used
- Windows Server with Active Directory
- Active Directory Users and Computers (ADUC)
- Group Policy Management Console (GPMC)
- File Explorer for managing file system security

## Steps to Execute the Project

### 1. Launch Active Directory Users and Computers (ADUC)
I started by launching ADUC from the Windows Server, which is the primary tool used for managing Active Directory objects. This tool allowed me to create and manage the various organizational units, users, and groups required for the project.

### 2. Create OU Structure
Using ADUC, I created a top-level Organizational Unit (OU) named `Student Union Department`. Within this OU, I created sub-OUs for different units, such as `Unit1` and `Unit2`. This hierarchical structure is essential for efficiently managing and applying policies to different groups within the organization.

![Create OU Structure]
*Screenshot Explanation: This screenshot shows the OU hierarchy in Active Directory, with the `Student Union Department` as the parent OU and `Unit1` and `Unit2` as sub-OUs.*

### 3. Add Users to OUs
Next, I added users to the OUs, creating at least two users per unit OU. This involved defining user attributes and ensuring they were correctly placed within their respective units. Managing users in Active Directory allows for centralized administration of network resources and user permissions.

![Add Users to OUs]
*Screenshot Explanation: This screenshot displays the user accounts created within each OU, highlighting their placement and attributes.*

### 4. Establish Groups Within Each OU
Following user creation, I established necessary groups within each OU. Grouping users simplifies permission assignments and policy applications. Each unit's groups were created under their respective OUs, and additional groups were created under the Student Union department OU.

![Establish Groups]
*Screenshot Explanation: This screenshot shows the groups created within each OU, demonstrating the organized structure for managing permissions.*

### 5. Mirror OU Structure in File System
To reflect the OU structure in the file system, I created a file system hierarchy that mirrored the OU setup. This structure ensures that directory access and permissions align with the organizational hierarchy. I then applied share and file system permissions specific to each unit’s directories.

![Mirror OU Structure]
*Screenshot Explanation: This screenshot depicts the file system structure that mirrors the OU hierarchy, showing the applied permissions.*

### 6. Apply Group Policy to Disable RUN Command
I launched the Group Policy Management Console (GPMC) to manage and apply Group Policies. I created a GPO to disable the RUN command for Student Union Student Assistants. This policy was carefully linked to the appropriate OUs to ensure it did not affect full-time employees or Domain Admins.

![Apply Group Policy]
*Screenshot Explanation: This screenshot displays the GPO settings and the linkage to the specific OUs, illustrating the targeted application of the policy.*

### 7. Verify Group Policy Application
Finally, I verified that the Group Policy was correctly applied. This involved testing the policy on affected user accounts to ensure the RUN command was disabled for Student Assistants while remaining accessible to full-time employees and Domain Admins.

![Verify Group Policy]
*Screenshot Explanation: This screenshot shows the results of the policy verification process, confirming that the RUN command is disabled for Student Assistants.*

## Results
- Successfully implemented an OU hierarchy and corresponding file system structure.
- Established effective user and group management within Active Directory.
- Applied targeted Group Policy to manage user permissions and enhance security.

This project showcases my skills in managing Active Directory, implementing organizational structures, applying security policies, and ensuring effective user and group management.

[Mohammad Faal-AD-POC.pdf](https://github.com/user-attachments/files/15773827/Mohammad.Faal-AD-POC.pdf)
