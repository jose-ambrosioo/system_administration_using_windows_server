# system_administration_using_windows_server
(WINDOWS SERVER | WINDOWS | VMWARE WORKSTATION | VIRTUALIZATION)

Implemented a scalable network infrastructure tailored to the company's business volume, ensuring flexibility and efficiency, and ensuring that branch users had the same working conditions and performance as head office users.

Configured the following services: AD DS, DNS, DFS, DHCP, FTP, IIS, Storage File Server, Failover Cluster, O and P Drive Server.

Requirements for Headquarters (Luanda state) and Branch (Benguela state) servers and switches:
- IP Address Configuration
- Server 1 (Windows Server 2019), Services Configuration: AD DS, DNS, DFS, Storage File Server, O and P Drive Server.
- Server 2 (Windows Server 2019), Services Configuration: DHCP, FTP, IIS, Failover Cluster.
- Clients (Windows 7, 8, or 10), Dynamic/Static IP Assignment from DHCP.
- Installation of BG Info on Server 1, Server 2 and Clients.

Configured services:
- Configured the Company Domain (Headquarters and Branch).
- Configured the OU in each site (Headquarters and Branch), with its own structure to store its objects.
- Configured department objects in the OU.
- Configured groups in the OU.
- Created user accounts to be able to log into Luanda and Benguela.
- Restricted access to the system in a certain period of the day and days of the week.
- Created administrator accounts (normal and administration) that have access to all servers and insertion in a group.
- Configured P:Drive for each user, to store automatically mapped personal data.
- Configured Dropbox with read and write permission to share data from all users.
- Restricted access to department folders allowing only members to have access to their department's folder, except DG members who have access to folders in all departments.
- Configured company websites available via IIS.
- Configured the company's FTP with access restricted to members of a group.

Security:
- Infrastructure security is managed in the OU via GPO for computers and users.

**AD DS**
